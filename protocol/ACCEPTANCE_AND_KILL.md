# BAT-VAL-001 acceptance and kill criteria

**ADVISORY RESEARCH SYSTEM — NO CONTROL AUTHORITY**

Protocol BAT-VAL-001 1.0.0. Pre-registered 2026-10-13.
Protocol object SHA-256: `6162d17e0e0f65754c3944560842efbb1a97390921bd217394defe2506032d8a`.
Live outcome: BLOCKED_PHYSICAL_EVIDENCE_REQUIRED. Technology gate: CLOSED.

## Accept only if all of these are true

- Qualifying structure in the protocol is complete.
- Late-band (20–80 s) mean residual is positive.
- That residual is greater than max(3 × combined standard uncertainty, 5 mV).
- At least 3 windows per cell, at least 3 cells, at least 2 lots.
- Reproduced across cells and across lots.
- It does not disappear on the improved-measurement repeat.
- No alternative-cause row is "explains".
- Failed runs are still in the hashed record.

## Kill, downgrade, or reclassify if

- It disappears under improved measurement.
- It is not reproducible across qualifying cells.
- It does not survive the second lot.
- It tracks temperature or another controlled variable.
- Contacts, wiring, the instrument, the cycler, sampling, current error, or rest current account for it.
- SOC mismatch accounts for it.
- A 3-time-constant relaxation, or cell/lot variation, accounts for it.
- The residual does not clear the locked floor.

Do not lower the floor, drop a lot, or delete a run after seeing the numbers. A changed rule is a different protocol and a different hash.

These criteria do not mention nickel, Ω CELL, AVA-BATT, or AVA-NEXUS, and they must not be edited to add them.
