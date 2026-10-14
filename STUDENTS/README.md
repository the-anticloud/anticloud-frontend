# Students — FRONTEND

**Project:** FRONTEND  
**Category:** CONSUMER_APPLIANCES  
**Upstream:** https://github.com/home-assistant/frontend  
**Pinned commit:** `24c3ab6061708c357d9836948302521086ddeb06`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `ed4caac90184118ad9e4161799cc6d612eed6252934c311089bcd3664705f64c`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `24c3ab6061708c357d9836948302521086ddeb06`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `ed4caac90184118ad9e4161799cc6d612eed6252934c311089bcd3664705f64c`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
