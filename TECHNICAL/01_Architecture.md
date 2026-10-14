# Technical Architecture — FRONTEND

**Upstream:** [https://github.com/home-assistant/frontend](https://github.com/home-assistant/frontend)
**License:** Apache 2.0
**Category:** CONSUMER_APPLIANCES
**Anticloud Integration:** PAX L5 Narrow L2 General 27B + AIOSS + Offline-First

## Upstream Description

HA dashboard for appliance control

## Anticloud Architectural Changes

1. PAX L5 Narrow L2 General 27B local voice assistant replacing cloud voice APIs
2. Single-binary firmware update package with AIOSS-verified integrity
3. AES-256 encryption for all usage telemetry stored on-device
4. Zero-cloud operation mode: full functionality without internet connectivity
5. Local energy optimization inference replacing cloud energy management APIs
6. GPU/CPU equalizer: inference scales to embedded ARM or x86
7. AIOSS audit chain for all firmware updates and configuration changes
8. Open CLI for configuration replacing proprietary mobile app requirement

## Integration Points

- **PAX Inference Socket:** Local HTTP endpoint at `127.0.0.1:11434/v1/chat` — same OpenAI-compatible API, zero cloud
- **AIOSS Hook:** Every write operation calls `aioss_append(event, payload)` before commit
- **Encryption Layer:** All file I/O routed through `anticloud_crypto.encrypt_at_rest()`
- **Single Binary Build:** `pyinstaller anticloud_frontend.spec` or `go build -o frontend`

## Deployment Modes

| Mode | Hardware | Notes |
| --- | --- | --- |
| Edge CPU | Raspberry Pi 4 / Intel NUC | Full feature set, PAX on CPU |
| Desktop GPU | RTX 3060 / A10 | PAX GPU inference, <1s latency |
| Server | 2× A100 | Full batch throughput |
| Air-gapped | Any x86/ARM | Zero network dependency |