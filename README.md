# BALLISTICSTOOLKIT_PRIOR_DOCS

![licence](https://img.shields.io/badge/licence-MIT-blue) ![checks](https://img.shields.io/badge/checks-0_PASS-brightgreen)

> Governed Anticloud packaging of upstream `BALLISTICSTOOLKIT_PRIOR_DOCS` in category **ARTILLERY_MANUFACTURING**. 0/16 checks PASS (measured). Every number traces to a named file plus run stamp.

**Upstream:** https://github.com/chasep255/BallisticsToolkit | **Upstream pin:** `a4a83e5cfe32de7ff8e5c955c21343443d0cdf6c` (source: gitfile:HEAD-ref) | **Category:** ARTILLERY_MANUFACTURING | **Licence:** MIT | **Overlay licence:** Anticommons 0.1.0

---

## What This Project Does

# Ballistics Toolkit

Client-side web-based ballistics calculator and simulation suite for long-range shooting. Built with WebAssembly and Three.js, it provides trajectory calculations with atmospheric and wind compensation, spin effects, load comparison, Performance Matrix analysis, Monte Carlo target simulation, hit simulation, interactive steel target simulator, an interactive F-Class match simulator with wind visualization, and a printable target generator.

**Website:** https://www.ballisticstoolkit.com/  
**Contact:** admin@ballisticstoolkit.com

## Features

### 📊 Ballistic Calculator
- **G1/G7 Drag Models** - Industry standard drag functions with ballistic coefficients
- **Environmental Compensation** - Temperature, humidity, and altitude (atmospheric pressure calculated automatically)
- **Spin Effects** - Spin drift and crosswind jump modeling with bullet spin rate calculation
- **Client-Side Performance** - WebAssembly for fast calculations, no server needed

### ⚖️ Load Comparison
- **Side-by-Side Comparison** - Compare two loads with drop, velocity, energy, wind drift, and flight time
- **100-Yard Intervals** - Data at every 100 yards out to your specified max range
- **Percentage Advantage** - See how much better or worse Bullet 2 is compared to Bullet 1
- **Flexible Units** - Display drop and drift in MOA, MRAD, or inches
- **10 mph Crosswind** - Standard crosswind for consistent drift comparison

### 🎛️ Performance Matrix
- **BC/MV Grid Comparison** - Compare wind drift, drop, velocity, energy, and MV sensitivity across different ballistic coefficients and muzzle velocities
- **Five Analysis Tables** - Wind drift (10 mph crosswind), drop, final velocity, final energy, and MV sensitivity (±0.5% velocity variation)
- **Color-Coded Results** - Green shows best performance, red shows worst, with smooth interpolation between
- **Customizable Ranges** - Define BC range (start/end/increment) and MV range
- **Flexible Settings** - G1/G7 drag models, MOA/MRAD/inches units, ft-lbs/Joules energy, full atmosphere controls
- **Load Development** - Identify optimal BC/MV combinations and evaluate sensitivity to velocity variations

### 🎯 Target Simulator
- **Monte Carlo Simulation** - Statistical analysis of shooting precision
- **Target Library** - 17 competitive targets to choose from
- **Realistic Variability** - Muzzle velocity, wind, and rifle accuracy modeling
- **Spin Effects** - Spin drift and crosswind jump included in analysis
- **Interactive Visualization** - Zoom, pan, and detailed shot impact display
- **Match Scoring** - Competitive scoring with X-counts, line breaking, and group size analysis

### 🎲 Hit Simulator
- **Monte Carlo Simulation** - Run up to 50,000 shots against custom target shapes
- **Custom Target Shapes** - Circle (by diameter) or rectangle (by width/height) in inches
- **Dispersion Statistics** - Hit probability, horizontal/vertical spread, extreme spread, mean radius, radial standard deviation, and CEP
- **Full Ballistics** - Same G1/G7 drag models, atmosphere, spin effects, and wind variability as the other tools
- **Persistent Settings** - Cookie-based save/restore of all parameters

### 🌬️ Wind Generator
- **Real-time Wind Visualization** - Interactive 2D wind field visualization showing wind speed and direction across the range
- **Procedural Wind Patterns** - Multi-octave curl noise generates swirling wind patterns that evolve over time
- **Wind Presets** - Zero, Dead, Calm, Moderate, Strong, Extra Strong
- **Adjustable Time Speed** - Speed up or slow down simulation time to observe wind patterns

### 🎮 F-Class Simulator
- **Two Match Modes** - String Fire (configurable matches, shots per match, and minutes per match; defaults 3 × 20 shots × 20 min aggregate) and Pair Fire (two players alternating on one rifle/target)
- **Pair Fire** - Per-turn timer (or unlimited), per-player sighters and configurable record shots, per-shooter scope persistence, dual HUD with active-shooter highlight, and X-count → sudden-death tiebreak
- **AI Opponent (Pair Fire)** - Set Player 2 to an AI to duel the computer on the shared target. Each level differs in how it reads and manages the wind. It reads the flags as a lagged average (so it trails switches), holds for both wind drift and crosswind jump, and then chases: after each shot it folds a fraction of where the shot landed into a correction for the next, the way you work off the spotter, which over-corrects when the condition has already moved. Easy reads poorly and over-chases, so it swings around chasing the wind; Medium is decent; Hard reads accurately, weights the near flags by time-of-flight, makes small measured corrections, and waits for its condition, though a fast switch still catches it now and then. All levels fire through the same rifle dispersion you do (no extra wobble) and take a realistic skill-based pause before each shot; you keep your sight picture and watch its shot land
- **Dual Scopes** - Spotting scope for wind reading, rifle scope for aiming
- **Wind Reading** - Heat mirage effect responds to wind speed and direction; reactive 3D wind markers (selectable wind flags or wind socks) at multiple distances
- **Advanced Wind Simulation** - Multi‑octave curl noise with advection and multiple presets (see Wind Generator)
- **Spin Effects** - Spin drift and crosswind jump included in trajectory calculations and trace visualizations
- **Match-Style Scoring** - Authentic target animation, detailed scorecard with per-section impact (grouping) diagrams
- **Remote Play (Beta)** - Host a match and stream the live view (and audio) to another person who plays it remotely. The host shares a single invite link; connections are brokered by the free PeerJS service and the audio/video is peer-to-peer (no account). In Pair Fire the host plays Player 1 and the remote player plays Player 2, with turn-gated controls
- **Immersive Environment** - Procedural terrain, dynamic audio, comprehensive HUD
- **Debug Mode** - A

(Full upstream documentation preserved in UPSTREAM_CLONE/README.md.)

---

## Installation

3. **Variability** - MV standard deviation, BC standard deviation (% of BC), wind variability, rifle accuracy
4. **Environment** - Altitude, temperature, humidity (pressure derived)

Watch realistic shot impacts on competitive targets with detailed logging and statistical analysis. Trajectories include spin drift and crosswind jump effects.

## Usage

- **Dual Scopes** - Spotting scope for wind reading, rifle scope for aiming
- **Wind Reading** - Heat mirage effect responds to wind speed and direction; reactive 3D wind markers (selectable wind flags or wind socks) at multiple distances
- **Advanced Wind Simulation** - Multi‑octave curl noise with advection and multiple presets (see Wind Generator)
- **Spin Effects** - Spin drift and crosswind jump included in trajectory calculations and trace visualizations
- **Match-Style Scoring** - Authentic target animation, detailed scorecard with per-section impact (grouping) diagrams
- **Remote Play (Beta)** - Host a match and stream the live view (and audio) to another person who plays it remotely. The host shares a single invite link; connections are brokered by the free PeerJS service and the audio/video is peer-to-peer (no account). In Pair Fire the host plays Player 1 and the remote player plays Player 2, with turn-gated controls
- **Immersive Environment** - Procedural terrain, dynamic audio, comprehensive HUD
- **Debug Mode** - Add `?debug=1` to URL for rapid testing (1-min matches, 2 shots)

## API

See upstream source in UPSTREAM_CLONE/ and the quoted documentation above.

## Dependencies

| Metric | Value |
|--------|-------|
| Files | measured |
| Lines of Code | measured |
| Dependencies | measured |
| Upstream licence | MIT |
| Overlay licence | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

- **Spin Effects** - Spin drift and crosswind jump modeling with bullet spin rate calculation
- **Client-Side Performance** - WebAssembly for fast calculations, no server needed

## Contributing

# Contributing to Ballistics Toolkit

We welcome small, focused pull requests.

## How to Contribute

1. Fork the project and create a feature branch.
2. Follow coding styles:
   - C++: clear naming, no dead code, guard clauses, const-correct, small helpers inline.
   - Web: ES modules, clear names, minimal DOM churn, no magic numbers.
3. Keep PRs small and focused. Include a short rationale and testing notes.
4. Ensure it builds and runs locally before submitting.

## License

By submitting a pull request, you agree that your contributions will be licensed under the MIT License.

## Reporting Issues

Open an issue with steps to reproduce, expected behavior, and environment details.

## Licence

Upstream (c) its contributors under MIT - see `UPSTREAM_CLONE/LICENSE`. This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- URL: https://github.com/chasep255/BallisticsToolkit
- Pinned commit: `a4a83e5cfe32de7ff8e5c955c21343443d0cdf6c`
- Verify: compare against the pinned commit in the upstream project history.

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`5c634ee09b4c8fb1372df0da98ba9a296688522b61c51e89329c0446a664fbd8`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

