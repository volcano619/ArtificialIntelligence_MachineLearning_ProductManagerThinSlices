# PRD — Driver Safety Copilot (Thin Slice) — v0.1
_Last updated: 2025-09-18 11:40:12 IST_

## 1. Problem
... (same as earlier) ...
## 7. Metrics & Current Results (v0.1)
**Classes:** `eyes_closed`, `phone_use`, `safe_driving`  
**Example run (balanced 32 labels / 31 preds):**

- eyes_closed → Precision **83.33%**, Recall **83.33%**, F1 **83.33%**
- phone_use → Precision **81.82%**, Recall **75.00%**, F1 **78.26%**
- safe_driving → Precision **75.00%**, Recall **85.71%**, F1 **80.00%**

**Averages:** Macro F1 **80.53%** | Micro F1 **86.21%**  
**Latency:** p95 **~329 ms** (✅ within <3,000 ms SLO)

Confusions: occasional `phone_use` ↔ `eyes_closed`, and `safe_driving` mis→`phone_use`.

**Prior run**: Macro F1 **87.5%**, Micro F1 **91.8%**, p95 **322 ms** (different mock distribution).

## Next Steps
- Expand to 100–150 windows, add real eye-state (mediapipe EAR) and gaze proxy.
