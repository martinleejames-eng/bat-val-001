# BAT-VAL-001 raw telemetry schema

**ADVISORY RESEARCH SYSTEM — NO CONTROL AUTHORITY**

Protocol BAT-VAL-001 1.0.0. Pre-registered 2026-10-13.
Protocol object SHA-256: `6162d17e0e0f65754c3944560842efbb1a97390921bd217394defe2506032d8a`.
Live outcome: BLOCKED_PHYSICAL_EVIDENCE_REQUIRED. Technology gate: CLOSED.

Required columns, one row per sample, immutable after the hash:

| Field | Unit | Rule |
|---|---|---|
| time_s | s | monotonic, one clock |
| cell_id | text | matches the allocation table |
| lot_id | text | withheld from the analyst until scoring is hashed |
| current_a | A | positive discharge |
| voltage_v | V | four-wire cell voltage |
| temp_c | °C | cell temperature |
| regime | text | pulse, rest, or other |
| window_id | text | rest window identifier |

Minimum rate 10 Hz through each rest. No gap fill. No smoothing in the raw file. A second file may hold derived residuals. It must point at the raw hash and must not replace it.
