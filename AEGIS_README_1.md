# 🛡️ AEGIS — Autonomous Engagement & Guidance Interception System

> **IEEE Student Competition 2025 — Preliminary Round Winner**  
> Team SkyNetra · Aerospace & Defense Technology Track · SDG 16

---

## What is AEGIS?

AEGIS is a physics-based drone threat interception simulation built entirely in the browser — no installation, no server, no dependencies. It models five real-world drone threat types and demonstrates how an autonomous AI interception engine detects, tracks, and neutralises them in real time.

This is not a game. It is a defense training and research tool built on real aerospace principles — proportional navigation guidance, radar cross-section modelling, and debris ballistics — made accessible to any institution in the world via a single URL.

---

## Why We Built This

Drone threats are one of the fastest-growing security challenges globally. Commercial drones costing a few hundred dollars are being weaponised in conflict zones worldwide. Existing defense systems were built for missiles, not slow, low-flying, low-RCS drone swarms. And training tools for counter-drone defense cost millions in infrastructure, live munitions, and restricted airspace.

AEGIS removes every one of those barriers. A defense instructor anywhere in the world can open this on a laptop and run a full threat simulation in under 30 seconds.

---

## Live Demo

Open `index.html` in any browser. No installation required.

Or visit the live hosted version:  
🔗 https://rohangupta214.github.io/aegis-drone-defense

---

## Features

### 5 Drone Threat Classes
Each with distinct flight behaviour, speed, payload, and radar cross-section:

| Threat Type | Behaviour | Challenge |
|---|---|---|
| Recon Drone | Slow, high altitude | Early detection |
| Kamikaze Drone | Fast, direct impact trajectory | Speed of intercept |
| Drone Swarm (×3) | Multiple simultaneous threats | Multi-target tracking |
| Loitering Munition | Circles before striking | Delayed engagement |
| Stealth Micro-Drone | Low RCS, hard to detect | Radar sensitivity |

### Physics Engine
- **Proportional Navigation Guidance** — the same intercept mathematics used in real missile systems
- **Radar Cross-Section (RCS) Modelling** — stealth drones are harder to detect and lock
- **Debris Ballistics** — intercept point is chosen to minimise ground damage from falling fragments
- **Layered Defense** — missed intercepts trigger an automatic secondary interceptor

### Real-Time Analysis
- Live threat risk score (0–100) with Safe / Warning / Critical zones
- Active drone telemetry — position, altitude, speed, phase, drone type
- Intercept record — kill zone, altitude at kill, intercept speed
- Debris fragment tracking
- AI event log with timestamps: Detect → Lock → Intercept → Contain

### Dual Simulation Mode
Split-screen comparison of AEGIS-engaged vs. no-defense scenario. Risk reduction is quantified in real time — showing exactly what the interception system prevents.

### Configurable Parameters
- Drone speed, payload weight, RCS signature
- Interceptor speed and engagement range
- Toggle: trajectory trail, radar sweep, debris field, threat heatmap, AI analysis

---

## Technical Architecture

```
Single HTML file — zero external dependencies
│
├── Physics Engine          Proportional navigation, RCS, debris ballistics
├── Radar Sweep Module      Angular sweep, threat blip detection, lock-on
├── Interception Logic      Intercept vector calculation, kill zone prediction
├── Threat Classifier       5 drone classes with distinct behavioural profiles
├── Dual-Sim Renderer       Canvas-based split simulation with live delta
└── AI Event Logger         Timestamped intercept chain log
```

**Stack:** Pure HTML5 + Canvas API + Vanilla JavaScript  
**Deployment:** Single file — runs in any browser, any device, offline  
**Dependencies:** Zero

---

## IEEE Competition

AEGIS was submitted to the **IEEE Student Competition 2025** under the Aerospace & Defense Technology track, aligned with **SDG 16 — Peace, Justice & Strong Institutions.**

- ✅ **Preliminary Round — Winner**
- 🌏 **Shortlisted for international presentation — Indonesia 2026**
- Team: **SkyNetra** — Rohan Gupta (Team Lead) & Aryan Gupta

---

## Roadmap

| Phase | What | Status |
|---|---|---|
| Phase 1 | 2D physics simulation, 5 threat classes, intercept engine | ✅ Complete |
| Phase 2 | 3D WebGL engine — Three.js port for spatial geometry | 🔲 Planned |
| Phase 3 | AI drone evasion — RL agent trains drones to evade | 🔲 Planned |
| Phase 4 | Real map integration — GPS overlay via Leaflet.js | 🔲 Planned |
| Phase 5 | Multi-layer defense — close, mid, and long-range tiers | 🔲 Planned |

---

## What I Learned Building This

- How **proportional navigation** works — the mathematics behind real missile intercept systems
- How **radar cross-section** affects detection probability for stealth aircraft
- How to build a **real-time physics simulation** using the HTML5 Canvas API
- How to structure a **multi-scenario simulation** with configurable parameters
- How to present technical defense research to an **IEEE panel**
- How engineering can directly serve **social good** — accessible tools for institutions that can't afford expensive training infrastructure

---

## Project Structure

```
aegis-drone-defense/
│
├── index.html        # Complete simulation — entire project in one file
└── README.md         # This file
```

---

## References

1. US Department of Defense (2023). *Counter-UAS Technology Assessment.* DoD Office of the Secretary of Defense.
2. Gettinger, D. (2023). *The Drone Databook.* Center for the Study of the Drone, Bard College.
3. Shaferman, V., & Shima, T. (2008). Unmanned Aerial Vehicles Cooperative Tracking of Moving Ground Target in Urban Environments. *Journal of Guidance, Control, and Dynamics, 31*(5).
4. Missile Defense Agency (2022). *Ballistic Missile Defense System Overview.* MDA Technical Report.
5. IEEE Standards Association (2021). *IEEE 2510-2021: Standard for Drone Risk Assessment in Urban Airspace.*

---

## Author

**Rohan Gupta**  
Class 12 Student | Jammu, India  
IEEE Student Competition 2025 — Preliminary Round Winner  

🔗 [GitHub Profile]github.com/RohanGupta214 
📧 rohangupta.8490@gmail.com

---

*Built for the IEEE Student Competition 2025. Physics engine, intercept logic, and simulation renderer written from scratch. No frameworks, no libraries — pure browser technology.*
