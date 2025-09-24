---
mode: 'agent'
description: 'Add coordinated arm movements to the hip countdown' 
---

# Step 3: Coordinated Arms

Enhance the Step 2 countdown by adding the arm motor (Port D) so hips, arms, and lights form a coordinated mini routine.

Only work in this file: `break_dance.py`.

Additions from Step 2:
1. Introduce `arm_pulse()` mirroring hip timing (smaller angles e.g. 70/80/90).
2. Modify countdown loop so each pulse triggers: sensor flash -> hip_pulse -> arm_pulse.
3. Keep per-number color scheme and increasing motion intensity.
4. Retain intro and final beep indicator.

Do NOT add beats (sound per pulse) yet beyond the existing final beep.

Acceptance criteria:
- Arms move on every pulse immediately after (or tightly with) hip motion.
- Angles scale per number group (e.g. bigger on 3 than on 1).
- Lights still flash each pulse.

Upload automatically after changes.

