# BAT-VAL-001 — Pre-Registered Physical Validation Protocol v1.0.0

**This is a pre-registration, not an announcement of a successful experiment.**

**NOT YET RUN / PHYSICAL EVIDENCE REQUIRED**

Technology gate: **CLOSED**

> We found a candidate signal. Instead of declaring a discovery, we froze the validation test before running it. The protocol is now public and hash-locked. The technology gate remains closed until physical evidence clears the pre-registered threshold.

## Locked identity

| Item | Value |
|---|---|
| Lab | 1.0.0 |
| Discovery Engine | 1.4.0 — frozen, not included in this record |
| Protocol | BAT-VAL-001 v1.0.0 |
| Protocol object SHA-256 | `6162d17e0e0f65754c3944560842efbb1a97390921bd217394defe2506032d8a` |
| BAT-VAL status | BLOCKED — PHYSICAL EVIDENCE REQUIRED |
| Technology gate | CLOSED |
| Physical measurements entered | NONE |
| Validation packet | EMPTY |
| Software checks of the protocol | 33/33 pass — these are not physical validation |

The protocol object hash above is the pre-registration lock. It is not a hash of these markdown files. File hashes are in `MANIFEST.sha256`.

## What was observed, and what is not a target

BAT-DISC-001 remains an unchanged discovery candidate:

- Evidence: SUPPORTED
- Repeatability: HIGH
- 7 of 8 envelope-valid windows
- Observed peak: 17.9 mV in the 20–80 s band
- Discovery score: 92%
- Three alternative causes: UNRESOLVED
- Technology: NOT PROVEN

**The 17.9 mV discovery observation is not the BAT-VAL-001 acceptance target.** Matching it is not required and is not sufficient.

## Pre-registered rule

A positive late-band residual must exceed:

`max(3 × campaign uncertainty, 5 mV)`

on at least 3 cells, from at least 2 lots, using four-wire (Kelvin) sensing, with traceable calibration, and with the raw experimental files SHA-256 hashed before scoring.

The decision tree and the acceptance and kill criteria are the files in `protocol/`. They are reproduced here without edits. Every measurement and result field is blank.

## Outcomes

- A. Failed to replicate.
- B. Explained or reclassified.
- C. Physically replicated — cause unresolved.

Outcome C permits further characterisation only. Outcome C does not establish chemistry, nickel, Ω CELL, AVA-BATT, AVA-NEXUS, commercial viability, or a new battery technology.

Simulations, EON predictions, discovery scores, human approval, and software tests do not constitute physical validation.

## What this record does not contain

No discovery-engine source, no dataset generator, no credentials, and no filled results. A future methodological change requires a new version and a new protocol hash. v1.0.0 stays at this tag.

NO PHYSICAL EVIDENCE = NO VALIDATION.

## Files

- [protocol/ACCEPTANCE_AND_KILL.md](protocol/ACCEPTANCE_AND_KILL.md)
- [protocol/ATTACK_MATRIX.md](protocol/ATTACK_MATRIX.md)
- [protocol/CELL_LOT_TABLE.md](protocol/CELL_LOT_TABLE.md)
- [protocol/DECISION_TREE.md](protocol/DECISION_TREE.md)
- [protocol/EQUIPMENT_CHECKLIST.md](protocol/EQUIPMENT_CHECKLIST.md)
- [protocol/EXPERIMENT_MATRIX.md](protocol/EXPERIMENT_MATRIX.md)
- [protocol/INTEGRITY.md](protocol/INTEGRITY.md)
- [protocol/METADATA_SCHEMA.md](protocol/METADATA_SCHEMA.md)
- [protocol/PROTOCOL.md](protocol/PROTOCOL.md)
- [protocol/RAW_TELEMETRY_SCHEMA.md](protocol/RAW_TELEMETRY_SCHEMA.md)
- [protocol/RELEASE_MANIFEST.md](protocol/RELEASE_MANIFEST.md)
- [protocol/REPORT_TEMPLATE.md](protocol/REPORT_TEMPLATE.md)
- [protocol/RUN_SHEET.md](protocol/RUN_SHEET.md)

Illustration, not the controlling text: [ARCHITECTURE.jpg](ARCHITECTURE.jpg)
