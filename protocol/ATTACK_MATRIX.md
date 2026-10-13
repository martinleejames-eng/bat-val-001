# BAT-VAL-001 alternative-cause attack matrix

**ADVISORY RESEARCH SYSTEM — NO CONTROL AUTHORITY**

Protocol BAT-VAL-001 1.0.0. Pre-registered 2026-10-13.
Protocol object SHA-256: `6162d17e0e0f65754c3944560842efbb1a97390921bd217394defe2506032d8a`.
Live outcome: BLOCKED_PHYSICAL_EVIDENCE_REQUIRED. Technology gate: CLOSED.

Each row must be filled with excluded, explains, or unresolved after a real test. Blank means the campaign is incomplete.

| Cause | How it is attacked | Result |
|---|---|---|
| Temperature | Arm T, and whether the residual tracks temperature inside the primary band | blank |
| Contact or lead resistance | Arm K, fixture swap, four-wire versus a deliberately bad sense | blank |
| Instrument / ADC | Arm M, second meter, range and filter settings | blank |
| Cycler behaviour | compare cell-terminal voltage with the cycler reading during rest | blank |
| Sampling | rate, gaps, aliasing, clock skew | blank |
| Current error | current zero and scale against a reference | blank |
| Residual rest current | windows with |I| ≥ 0.4 A are excluded, not scored | blank |
| SOC mismatch | Arm S | blank |
| Ordinary relaxation | frozen 3-time-constant fit; explains the band only if the late residual falls to or below the floor | blank |
| Cell variation | spread across the three cells | blank |
| Lot variation | lot A versus lot B | blank |
| Baseline-model inadequacy | this is the finding under test, not a technology | blank |

An ordinary explanation is a successful scientific result.
