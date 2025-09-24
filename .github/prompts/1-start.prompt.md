---
mode: agent
description: 'Start Break Dance robot - create basic MicroPython test program'
---

# Step 1: Create Basic Break Dance Robot

Create the basic Break Dancer program to verify connections and baseline functionality.

Only work in this file: `break_dance.py`.

The program should:
1. Display "DANCE" on the LED
2. Test arm movement (Port D) with proper motor control:
   - Initialize motor with `Motor(Port.D)`
   - Use `motor.run_angle(speed, rotation_angle)` to move arms in controlled movements
   - Test positive and negative rotations (e.g., 90 degrees forward, then back)
   - Use speed around 200 degrees/second for smooth movement
   - Add `wait()` between movements to see each motion clearly
   - Example: `arm_motor.run_angle(200, 90)` followed by `wait(500)`
   - Test both directions to ensure full range of motion
3. Test hip movement (Port F) with similar motor control:
   - Initialize motor with `Motor(Port.F)`
   - Use `motor.run_angle(speed, rotation_angle)` for hip movements
   - Test larger rotation angles (e.g., 180 degrees) for hip swaying motion
   - Use consistent speed (200 degrees/second) for synchronized movement
   - Add appropriate wait times between movements
   - Example: `hip_motor.run_angle(200, 180)` for hip sway
   - Return to center position after each test movement
4. Make the color sensor create rotating light patterns with individual brightness control (Port B)
   - The sensor has 3 built-in lights that can be controlled individually
   - Use `sensor.lights.on(brightness)` where brightness can be:
     * A single value (0–100%) to set all 3 lights to the same brightness
     * A tuple/list of 3 values `[light1, light2, light3]` to control each light individually (0–100% each)
   - Example: `sensor.lights.on([50, 0, 0])` turns on only the first light at 50% brightness
   - Example: `sensor.lights.on(100)` turns on all lights at maximum brightness
   - Use `sensor.lights.off()` to turn off all lights
   - Create a rotating chase effect cycling through the 3 lights with different brightness levels
   - Use different brightness combinations for dynamic visual effects
5. Play a beep using `hub.speaker.beep()`

After creating/updating the file:
- Recheck requirements vs. the generated code.
- Automatically upload it to the robot using the venv python and the name from `launch.json`.

Implementation notes (additive foundation):
- Keep code minimal; no choreography logic yet (that starts in later steps).
- Keep functions small and clear if you introduce any (optional at this stage).
