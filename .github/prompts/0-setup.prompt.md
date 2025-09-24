---
mode: 'agent'
description: 'Setup the project environment and test basic connection'
---

# Step 0: Project Setup

Set up the project environment properly before starting the dance robot development.

Tasks to complete:
1. Create and activate the Python virtual environment called venv by running the commands
2. Install the required dependencies (pybricksdev)
3. Test the robot connection with robot `robot_blink.py`, ALWAYS automatically upload it to the robot using the venv python and the name from launch.json.
4. Verify everything is working
5. Create an empty `break_dance.py` file if it does not exist

Follow the setup instructions in the README and ensure the correct Python environment is used for all uploads.

Implementation notes (additive & non-destructive):
- Create or update environment and dependency files only; preserve any existing source files and configuration.
- Verify the robot name in `.vscode/launch.json` and `README.md` and update them only if necessary.
- Do not change `robot_blink.py`


