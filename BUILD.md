# Building meow Wizard from Source

## Prerequisites

- Python 3.14+
- Windows (for the final EXE)

## Setup

```bash
# Install dependencies
pip install pyinstaller Pillow

# (Optional) Create a virtual environment
python -m venv venv
venv\Scripts\activate
pip install pyinstaller Pillow
```

## Build

```batch
pyinstaller --onefile --name meowWizard --add-data "static;static" --icon app.ico meow_wizard.py
```

> **Note:** The `static/` folder must exist in the same directory as `meow_wizard.py` at build time. It contains `index.html` (the frontend) and is not distributed publicly.

## After Build

The EXE will be at `dist/meowWizard.exe`. Copy it anywhere — it's fully portable.

## Run


A terminal opens with a local URL. Open it in your browser and follow the steps.
