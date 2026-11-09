Circuit Schematic Evolution – Interactive Graph & System Simulator
A lightweight, zero-dependency HTML5 Canvas interactive simulation engine that models system architecture evolution. The application visualizes how electrical and logical circuits scale from a basic single wire loop into a complex, modular telemetry and micro-robotics ecosystem with active wireless RF signal propagation.
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Tech Stack](https://img.shields.io/badge/tech-VanillaJS%20%7C%20HTML5%20Canvas%20%7C%20TailwindCSS-brightgreen)
---
Architecture Overview
This project was built to demonstrate core concepts in systems engineering, state machine management, and interactive data visualization without reliance on heavy framework overhead.
Key Architectural Highlights
State-Driven Directed Graph Engine: Custom state management mapping dependencies, component tiers, and prerequisites across dynamic nodes without framework dependencies.
Declarative Vector Symbol Rendering: Component schematics, active visual states, thermal particles, and signal traces are rendered dynamically via standard HTML5 Canvas 2D API context.
Vector Math & Coordinate Transformation: Integrated view-space transformation matrix handling smooth panning, infinite zooming, and screen-to-world coordinate translation for hover and click hit-testing.
Real-time Particle System & Physics Effects:
Signal Buses: Flowing electron pulse streams across independent traces (Power, Logic, Clock/PWM, High Voltage, Wireless RF).
Thermal Dissipation Dynamics: Convective particle emitters tied to node power tiers.
Wireless RF Propagation & Kinematics: Waveform propagation triggers mechanical servo tilt and force feedback sparks upon receiving control frames.
---
Logic Flow
```
[ Power Substation ] ─── (HV Bus) ───► [ Heatsinks & Protection ]
        │
        ├─── (Power Rail) ───────────► [ Dual-Bulb / Relay Loads ]
        │                                      │
[ Keypad Matrix ] ──► [ Demux Buffer ] ──► [ Discrete Logic / ALU ]
                             │                     │
                             ▼                     ▼
                     [ Clock Oscillator ] ──► [ Dual-Core MCU ]
                                                   │
                                                   ▼
[ Remote Telemetry Chassis ] ◄── (433MHz RF) ── [ PWM & RF Tx ]
        │
        ├──► [ HD Camera Optics & Vision Sensor ]
        └──► [ Quad MOSFET Driver ] ──► [ Steel-Gear Servo Actuators ]
```
---
Key Features
Zero-Dependency Core: Built purely with native JavaScript ES6+, HTML5 Canvas, and Tailwind CSS (UI overlays).
Interactive Node Evolution: Click to unlock and branch components. Dependencies enforce structured path discovery (e.g., Demux and Oscillator required prior to Microcontroller deployment).
Wireless Telemetry Pad: Unlocking the RF matrix reveals an active HUD controller capable of transmitting directional signals across the board gap to actuate chassis motors in real time.
Responsive Control Mechanics: Pinch-to-zoom, pan drag, hover diagnostic inspector cards, and adaptive canvas resizing.
---
Tech Stack
Frontend Engine: Vanilla JavaScript (ES6+), HTML5 Canvas API
UI & Overlay: Tailwind CSS, Fira Code (Monospace Engine Typography)
Design Pattern: Object-Oriented Component Rendering & Sub-system Graph Logic
---
How to run it
Because this project uses vanilla web standards, no node modules or build steps are required.
Clone the repository:
```bash
   git clone https://github.com/your-username/circuit-schematic-evolution.git
   ```
Open `index.html` directly in any modern web browser, or serve via standard static HTTP server:
```bash
   npx serve .
   ```
