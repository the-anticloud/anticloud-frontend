# Build and Test

**Project:** `FRONTEND`
**Upstream:** https://github.com/home-assistant/frontend
**License:** Apache 2.0

## Quick Start

```bash
git clone https://github.com/home-assistant/frontend
cd frontend
pip install -r requirements-anticloud.txt
python anticloud_main.py --offline --pax-local
```

## Anticloud Improvements Applied

1. PAX L5 Narrow L2 General 27B local voice assistant replacing cloud voice APIs
2. Single-binary firmware update package with AIOSS-verified integrity
3. AES-256 encryption for all usage telemetry stored on-device
4. Zero-cloud operation mode: full functionality without internet connectivity
5. Local energy optimization inference replacing cloud energy management APIs
6. GPU/CPU equalizer: inference scales to embedded ARM or x86
7. AIOSS audit chain for all firmware updates and configuration changes
8. Open CLI for configuration replacing proprietary mobile app requirement

## Benchmark Targets

| Metric | Target |
| --- | --- |
| Latency | Primary inference task: <5s on CPU, <1s on GPU |
| Throughput | Batch processing: >100 items/hour on single CPU server |
| Memory | <8GB RAM for standard deployment |
| Accuracy | Task-specific accuracy within 5% of cloud-API baseline |

## Build Status

Not yet measured. Run verified build and record actual figures above.
