# Model Card — Driver Safety Copilot (Thin Slice) — v0.1
_Last updated: 2025-09-18 11:40:12 IST_

## Current Performance (example balanced run)
Per-class: eyes_closed **83.33/83.33**, phone_use **81.82/75.00**, safe_driving **75.00/85.71** (P/R)  
Macro F1 **80.53%**, Micro F1 **86.21%**  
Latency p95 **~329 ms** (target < 3000 ms)

Risks: class confusion, synthetic data bias, privacy on real footage.
Mitigations: source evidence, “review” tag for low confidence, model version logging.
