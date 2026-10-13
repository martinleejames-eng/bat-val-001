# BAT-VAL-001 experiment matrix

**ADVISORY RESEARCH SYSTEM — NO CONTROL AUTHORITY**

Protocol BAT-VAL-001 1.0.0. Pre-registered 2026-10-13.
Protocol object SHA-256: `6162d17e0e0f65754c3944560842efbb1a97390921bd217394defe2506032d8a`.
Live outcome: BLOCKED_PHYSICAL_EVIDENCE_REQUIRED. Technology gate: CLOSED.

| Arm | What is held | What changes | Why | Status |
|---|---|---|---|---|
| P | 22–28 °C, declared SOC, 10 s 1C pulse, ≥ 120 s rest | cell and lot | replication | NOT RUN |
| T | same electrical profile | two temperatures outside 22–28 °C | temperature attack | NOT RUN |
| K | one cell | new fixture or Kelvin connection | contact and lead attack | NOT RUN |
| M | one window | second voltmeter | instrument attack | NOT RUN |
| S | same cell | a second pre-declared SOC | SOC-mismatch attack | NOT RUN |
| R | primary windows | none | ordinary 3-time-constant fit after the hash | NOT RUN |

An arm that is not run stays unresolved. It is not a pass.
