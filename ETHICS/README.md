# Ethics — BALLISTICSTOOLKIT_PRIOR_DOCS

**Project:** BALLISTICSTOOLKIT_PRIOR_DOCS  
**Category:** ARTILLERY_MANUFACTURING  
**Upstream:** https://github.com/chasep255/BallisticsToolkit  
**Pinned commit:** `a4a83e5cfe32de7ff8e5c955c21343443d0cdf6c`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `10b1fe73eeec07e7d31b79ddeae5c775dfe1480b9467343162267918a8890a25`  
**Date:** October 2026

## Position

BALLISTICSTOOLKIT_PRIOR_DOCS is packaged for offline deployment with a verifiable audit trail. The
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
