<p align="center">
  <img align="center" width="60%" height="60%" alt="official-nocturnal-rainbow-logo-dark-white-clouds" src="https://github.com/user-attachments/assets/673aa1ee-fae5-4c89-9fd0-31ebb6c8e196" />

  <p align="center">"<em>A modular, user-guided HID interface and key input surveillance framework for Windows, designed with clarity, stealth, and user-space control in mind.</em>"</p>
</p>

## 🔍 Summary:
<b>NocturnalRainbow</b> is a userland input instrumentation platform designed for advanced keyboard/mouse event monitoring, HID device inspection, and surface-level UI interaction tracing. It is built to serve as a prototype or skeleton for:

* Red team tooling.
* Device policy enforcement.
* Input analytics.
* Controlled telemetry collection.
* Low-level UX auditing.
* Reverse engineering of app-specific input behavior.

## 🧩 Core Features
* Configurable Input Capture Backend.
* Virtual keycode logging (via GetAsyncKeyState, GetKeyState, or raw input)
* Timestamped logging with optional modifier tracking (Ctrl/Alt/Shift)
* Optional clipboard capture or context-based filters.
* Switch between global hook vs. foreground polling.
* Device-Aware Monitoring.
* Enumerate HID keyboard-like devices (via SetupAPI or WMI)
* Allow user to exclude specific hardware paths (e.g., USB keyboards or Bluetooth HID)
* Tie captured input to specific device contexts where possible.
* Process-Level Awareness.
* Identify and display currently focused window, associated process, and thread ID.
* Allow user to limit logging to selected applications or window titles.
* Option to bind to child windows spawned by a process.

## UI/UX Layer:

* Lightweight GUI for toggling input sources, output modes, and key filters.
* Optional overlay that floats above windows, logs events in real-time.
* Transparent/ghost mode to avoid detection or visual clutter.
* Custom logging paths and formats (CSV, JSON, binary)
* Event Bus + Modular Hooks.

## Plug-in support for extensions like:

* Alerting on specific keys.
* Triggering macros/scripts on input.
* Screenshot on sensitive input.
* Built-in hotkey handler to pause/resume/toggle visibility.

## 🎯 Design Ethos
This tool reflects an operator mindset: it is not designed to be deployed at scale, but to give the developer full awareness, control, and strategic access to local input behavior across users, devices, and processes. The emphasis is on modularity, precision, and discretion, not mass surveillance or malware deployment.

## 🗂️ Use Cases (Legitimate)
* Auditing input devices in a sensitive environment (e.g., kiosk, server room)
* Detecting unauthorized HID injection (e.g., BadUSB or Teensy-style implants)
* Reverse engineering UI input flows in legacy software.
* Monitoring or debugging hotkey triggers in production environments.
* Creating a keystroke-controlled application launcher or productivity tool.

<br>

*Such power in the palm of your hands, brought to you by talent, all for free.*
