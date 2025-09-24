---
mode: 'agent'
description: 'Add LED countdown with synchronized hip pulses and sensor flashes' 
---

# Step 2: Hip Countdown Rhythm

Transform the basic test script into an early rhythmic prototype.

Only work in this file: `break_dance.py`.

Additions / Changes from Step 1:
1. REMOVE prior individual test functions for arms/hips/light chase.
2. Add a countdown (1,2,3) displayed on the hub.
3. For each number, perform that many hip pulses (Port F) using `run_angle` (increasing angle per number e.g. 140/160/180) returning to center each pulse.
4. Flash a sensor light pattern (Port B) per number (the light in the center does not have colors, only brightness controls). 
5. Keep the intro DANCE sequence and final beep.
6. Everything should be synchronized, make sure the next steps are not waiting for movements to finish before starting the next.

Constraints:
- Arm motor (Port D) is not yet active in this step (reserved for Step 3).
- Use helper functions: e.g. `countdown_hips()`, `hip_pulse()`, `flash_sensor()`.

Acceptance criteria:
- Countdown numbers appear clearly.
- Correct number of hip pulses per number.
- Light flashes accompany every pulse.
- Program ends cleanly with beep and OK (or similar) indicator.

Upload automatically with the canonical command using venv python.
