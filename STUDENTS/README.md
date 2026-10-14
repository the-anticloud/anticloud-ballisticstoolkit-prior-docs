# Students — BALLISTICSTOOLKIT_PRIOR_DOCS

**Project:** BALLISTICSTOOLKIT_PRIOR_DOCS  
**Category:** ARTILLERY_MANUFACTURING  
**Upstream:** https://github.com/chasep255/BallisticsToolkit  
**Pinned commit:** `a4a83e5cfe32de7ff8e5c955c21343443d0cdf6c`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `10b1fe73eeec07e7d31b79ddeae5c775dfe1480b9467343162267918a8890a25`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `a4a83e5cfe32de7ff8e5c955c21343443d0cdf6c`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `10b1fe73eeec07e7d31b79ddeae5c775dfe1480b9467343162267918a8890a25`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
