# BAT-VAL-001 integrity and hash procedure

**ADVISORY RESEARCH SYSTEM — NO CONTROL AUTHORITY**

Protocol BAT-VAL-001 1.0.0. Pre-registered 2026-10-13.
Protocol object SHA-256: `6162d17e0e0f65754c3944560842efbb1a97390921bd217394defe2506032d8a`.
Live outcome: BLOCKED_PHYSICAL_EVIDENCE_REQUIRED. Technology gate: CLOSED.

1. Stop the cycler under human control. Export raw files.
2. Do not open them in a tool that rewrites timestamps or interpolates.
3. Compute SHA-256 of each raw file. Hex, lowercase.
4. Write those hashes into the metadata, then hash the metadata.
5. Only then compute late-band residuals.
6. Hash the residual table before lot labels or historical names are restored.
7. Append every step to the laboratory audit. A missing hash means that step did not happen.
8. If a file is replaced, keep the old hash and add the new file. Do not pretend they are the same run.

Contradictory runs are hashed too. Dropping one is an invalid audit, not a cleaner result.
