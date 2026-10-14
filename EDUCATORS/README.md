# Educators — BALLISTICSTOOLKIT_PRIOR_DOCS

**Project:** BALLISTICSTOOLKIT_PRIOR_DOCS  
**Category:** ARTILLERY_MANUFACTURING  
**Upstream:** https://github.com/chasep255/BallisticsToolkit  
**Pinned commit:** `a4a83e5cfe32de7ff8e5c955c21343443d0cdf6c`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `10b1fe73eeec07e7d31b79ddeae5c775dfe1480b9467343162267918a8890a25`  
**Date:** October 2026

## Teaching with BALLISTICSTOOLKIT_PRIOR_DOCS

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `10b1fe73eeec07e7d31b79ddeae5c775dfe1480b9467343162267918a8890a25` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
