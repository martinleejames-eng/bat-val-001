# BAT-VAL-001 protocol

**ADVISORY RESEARCH SYSTEM — NO CONTROL AUTHORITY**

Protocol BAT-VAL-001 1.0.0. Pre-registered 2026-10-13.
Protocol object SHA-256: `6162d17e0e0f65754c3944560842efbb1a97390921bd217394defe2506032d8a`.
Live outcome: BLOCKED_PHYSICAL_EVIDENCE_REQUIRED. Technology gate: CLOSED.

## Purpose

Give the sealed rest-voltage signature a fair chance to survive independent physical attack, or to be killed by that evidence.

This protocol is not a plan to prove AVA EON, a chemistry, or a named cell correct.

The sealed discovery is context, not a target. The reported 17.9 mV peak is not required and is not sufficient.

## Frozen discovery context

- Finding: unmodelled post-load voltage recovery signature
- Evidence: SUPPORTED
- Repeatability: HIGH
- Windows: 7/8 envelope-valid
- Band: 20–80 s
- Technology: NOT_PROVEN

Discovery engine 1.4.0 stays frozen. This protocol does not change its score.

## What a qualifying campaign is

- Calibrated battery cycler. The laboratory does not hand control to this software.
- True four-wire (Kelvin) voltage sense at the cell terminals.
- Traceable calibration records and the full fixture configuration.
- At least 3 cells from at least 2 lots.
- Sampling at least 10 Hz, synchronized current, voltage, cell temperature, and time.
- Raw telemetry preserved unchanged, with a SHA-256 recorded before interpretation.
- Temperature controlled. Primary comparison band 22–28 °C.
- SOC, load history, and rest declared before the arm is run.
- Rest at least 120 s. A window counts only if |I| < 0.4 A.
- Primary pulse: one 10 s discharge at 1C, then open-circuit rest. Cell voltage limits come from the cell datasheet. If those limits are missing, the arm is blocked. This protocol does not invent them.
- Conditioning, written before data: two C/3 cycles between the datasheet voltage limits, then 30 min rest, then coulomb-count to the pre-declared SOC.
- Repeat windows: at least 3 envelope-valid rests per cell.
- Blinding: the analyst who scores the late-band residual does not receive lot labels or any historical EON design name until the residual table is hashed.
- Failed, null, and contradictory runs stay in the file. Deleting them makes the audit invalid.

## Acceptance

The late-band mean residual versus the frozen first-order baseline must be positive and greater than max(3 × combined standard uncertainty, 5.0 mV).

The floor uses the campaign's own uncertainty. It is not moved after the data are seen. Matching the synthetic peak is not a criterion. Discovery score, simulation, EON prediction, and human approval are not inputs.

## Outcomes

- A. Failed to replicate.
- B. Explained or reclassified by an ordinary cause.
- C. Physically replicated, cause unresolved.

Only C may proceed to characterisation. C does not establish new battery chemistry, nickel causation, Ω CELL, AVA-BATT, AVA-NEXUS CELL, commercial battery technology, improved battery performance, patentable technology.

## Live status

No physical packet is on file. Outcome: BLOCKED_PHYSICAL_EVIDENCE_REQUIRED.
