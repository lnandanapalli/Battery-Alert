# Battery Monitoring System

Minimal cross platform battery monitor script written in Python.  
It beeps and pops up a small Tkinter window when your laptop battery drops below a user defined **low** threshold or rises above a **high** threshold while still plugged in.

---

## Requirements

-   Python 3.7 or newer
-   Tkinter (bundled with standard CPython installs)
-   `psutil` Python package

Install the dependency:

    pip install -r requirements.txt

---

## Usage

Run the script and enter two integer thresholds:

    python3 battery_monitor.py
    Enter lowest battery percentage : 20
    Enter highest battery percentage : 90

-   Below **20 %** while on battery, beeps + shows Low battery window.
-   Above **90 %** while still plugged in, beeps + shows Charged window.

### Launchers

-   Linux/macOS: make executable and run

          chmod +x battery_monitor.sh
          ./battery_monitor.sh

-   Windows:

          battery_monitor.bat

Both wrappers invoke the Python script.

---
