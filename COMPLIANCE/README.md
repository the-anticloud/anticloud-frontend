# Compliance — FRONTEND

**Project:** FRONTEND  
**Category:** CONSUMER_APPLIANCES  
**Upstream:** https://github.com/home-assistant/frontend  
**Pinned commit:** `24c3ab6061708c357d9836948302521086ddeb06`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `ed4caac90184118ad9e4161799cc6d612eed6252934c311089bcd3664705f64c`  
**Date:** October 2026

## Position

FRONTEND is mapped against eleven frameworks in `BENCH.json`:
OWASP LLM Top 10, OWASP Top 10 (2021), SOC 2 Type II readiness, NIST AI RMF,
NIST SP 800-53 Rev. 5, NIST CSF 2.0, FedRAMP Rev. 5, PCI DSS v4.0.1,
ISO/IEC 27001:2022, MITRE ATT&CK v16, and ML TRL.

**Current result: 16/16 checks passing.**

## What the mapping asserts

For each framework, every in-scope control is bound to a named evidence source
in this project, and that source exists and is re-runnable. The control counts
and evidence counts are recorded per framework in `BENCH.json`.

## What is not claimed

No audit opinion, SOC report, FedRAMP authorisation, PCI attestation or ISO
certificate is held. Those are issued by an independent assessor against a
defined period of operation; no project can self-issue one. See
`OFFICIAL_BENCHMARKS/` for the per-framework scope statement.

## Verification

Open `ISOLATED_LAB_RESULTS/03_Result_Register.md`, read a row, recompute the
SHA3-256 of its evidence file in `04_Evidence/`, compare.
