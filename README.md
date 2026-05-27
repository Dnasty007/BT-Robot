# BT Robot Project

**BT** is our custom-built tiny all-terrain wheel-legged hybrid camera robot — the ultimate personal sidekick for cinematic auto-follow, dynamic jumps, flips, balance on rough terrain, and smart autonomous filming.

### 🎯 Goal: Match (and beat) Mondorobotics Beni
We discovered [Mondorobotics.com](https://mondorobotics.com/) and their flagship robot **Beni** is *exactly* the vision for BT:
- Tiny form factor (~8.5 × 7.1 × 7.1 in, ~3.86 lbs)
- Wheel-legged hybrid: high-speed wheels + legs for 10" jumps, stairs, rough terrain
- Dynamic balance, autonomous jumps, mid-air flips/somersaults, self-righting
- 4K camera with auto cinematic tracking, orbit shots, highlight auto-editing
- ~1.5 hr swappable battery

Beni is currently pre-launch. **$10 reservation locks in ~$500 early-bird pricing** on Kickstarter (highly recommended as a mechanical reference unit).

**Our strategy**: 
- Buy one Beni on day one for teardown + exact 3D-scan/clone of chassis, leg geometry, drivetrain.
- Use **open-source control stack** from their own CTO (Shuo Yang, ex-Tesla Optimus) instead of trying to hack the closed proprietary firmware.
- Layer our local LLM stack (Ollama/NemoClaw + hyTopia automation) for even smarter high-level reasoning.

This hybrid approach gives us full mechanical fidelity + superior hackability and AI smarts.

### 🛠️ Software Stack (the real magic — already ours)
- **Low-level control & balance/jumps**: A1-QP-MPC-Controller + Cerberus VILO (Visual-Inertial-Leg Odometry) — open-sourced by Shuo Yang.
- **Dynamic behaviors & acrobatics**: Reinforcement Learning policies (sim-to-real) for flips/self-righting.
- **Perception & autonomy**: DiT4DiT Vision-Action Model (MIT licensed) for real-time vision → action decisions.
- **High-level brain**: Our local LLMs for cinematic decision-making ("film the skate trick from this angle").

Beni's shipped firmware is locked/closed-source (no SDK or root expected). We don't need it — we already have better, fully open foundations.

### 📦 Parts & Build Cost (first functional prototype)

| Category              | Est. Cost     | Notes |
|-----------------------|---------------|-------|
| Actuators & Motors    | $800–$1,800  | 4–6 high-torque quasi-direct-drive servos (20–40 Nm) — CubeMars / ODrive style |
| Wheels & Drivetrain   | $150–$300    | Quick-swap treaded + smooth sets |
| Chassis & Legs        | $200–$500    | Aluminum/carbon + 3D-printed (Blender modeled after Beni) |
| Compute + Sensors     | $600–$1,200  | Jetson Orin Nano + IMU + 4K camera + optional LiDAR |
| Battery & Power       | $150–$300    | Swappable 1.5 hr+ packs |
| Misc (ESCs, wiring)   | $100–$400    | Tools + breakage buffer |
| **Total**             | **$2,000–$4,500** | Significantly cheaper long-term than multiple Benis |

### ⏳ Timeline
**6-month realistic target** for a fully functional Beni-level BT:
- Months 1–2: Design + simulation (Blender + Isaac Lab/MuJoCo)
- Months 3–4: Hardware assembly + basic MPC balance/jumps
- Months 5–6: RL training, cinematic autonomy, full testing

Expect iteration and broken parts — standard robotics journey.

### Status & Next Steps
- Beni reservation: $10 today locks $500 unit (teardown reference)
- Open-source repos from Shuo Yang already bookmarked
- Blender chassis template ready
- Shopping list + actuator links coming next

**BT isn't just a clone — it's our custom, fully open, AI-supercharged version.** Let's build the legendary one.

---

*Last updated: May 27, 2026*