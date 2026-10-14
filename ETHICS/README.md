# Ethics — FRONTEND

**Project:** FRONTEND  
**Category:** CONSUMER_APPLIANCES  
**Upstream:** https://github.com/home-assistant/frontend  
**Pinned commit:** `24c3ab6061708c357d9836948302521086ddeb06`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `ed4caac90184118ad9e4161799cc6d612eed6252934c311089bcd3664705f64c`  
**Date:** October 2026

## Position

FRONTEND is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
