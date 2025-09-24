---
mode: 'agent'
description: 'Add musical beats to the coordinated countdown' 
---

# Step 4: Add Beats

Extend the coordinated hips+arms+lights countdown by adding audio beats (tones) synchronized with each pulse.

Only work in this file: `break_dance.py`.

Additions from Step 3:
1. For each pulse, play a tone (e.g. ascending pitches A4, C5, E5 per count group).
2. Keep existing motion and light timing logic unchanged.
3. Retain intro and final OK (or beep) indicator.

Suggested helper: `coordinated_countdown(play_beats=True)`.

Acceptance criteria:
- Distinct audible pitch per number group.
- No regression of arm/hip/light behavior from Step 3.
- Beats trigger with each pulse.

Upload automatically after implementing.
