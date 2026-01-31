# Swarm Coder: AI Governance Through Geometry

**One-liner:** The navigation system for AI agents - the same math that coordinates drone swarms now coordinates coding agents.

---

## The Problem

AI agents are **blind boxes that run code**. They can't see:
- The full codebase
- What other agents are doing
- When they're drifting from intended behavior

Just like a drone without a camera needs sonar, GPS, and swarm awareness to avoid crashing - AI coding agents need governance, consensus, and spatial awareness to avoid errors.

---

## The Solution: 6 Agents, 1 Geometry

```
┌────────────────────────────────────────────────────┐
│                  SWARM CODER                       │
│   "6 AI agents that code like a drone swarm"       │
├────────────────────────────────────────────────────┤
│                                                    │
│    ┌─────┐    ┌─────┐    ┌─────┐                  │
│    │ KO  │    │ AV  │    │ RU  │  ← Design/Code   │
│    │Flow │    │I/O  │    │Policy│                 │
│    └──┬──┘    └──┬──┘    └──┬──┘                  │
│       │          │          │                      │
│       └──────────┼──────────┘                      │
│                  ▼                                 │
│       ┌──────────────────┐                         │
│       │  Poincaré Ball   │  ← Shared behavior     │
│       │  (Hyperbolic     │     space where        │
│       │   geometry)      │     position = intent  │
│       └──────────────────┘                         │
│                  ▲                                 │
│       ┌──────────┼──────────┐                      │
│       │          │          │                      │
│    ┌──┴──┐    ┌──┴──┐    ┌──┴──┐                  │
│    │ CA  │    │ UM  │    │ DR  │  ← Test/Verify   │
│    │Comp │    │Sec  │    │Auth │                  │
│    └─────┘    └─────┘    └─────┘                  │
│                                                    │
└────────────────────────────────────────────────────┘
```

---

## How It Works

### 1. Decimal Drift Detection
Every agent's actions are tracked as a position in hyperbolic space:

```
Agent drifts:  (0.2, 0.5) → (0.4, 0.6) → (0.7, 0.8)
Distance grows: 0 → 0.2 → 0.6

System response:
├── 0.0-0.3: Normal operation
├── 0.3-0.6: Increased scrutiny
└── 0.6+:    Require approval / DENY
```

### 2. Harmonic Wall Cost
The further you drift, the exponentially harder it gets:

```
H(d) = exp(d²)

d = 0.0  →  H = 1.00   (free)
d = 0.5  →  H = 1.28   (slight friction)
d = 1.0  →  H = 2.72   (noticeable)
d = 2.0  →  H = 54.6   (expensive)
d = 3.0  →  H = 8,103  (blocked)
```

### 3. BFT Consensus
4-of-6 agents must agree. One rogue agent can't corrupt the swarm.

---

## Technical Specs

- **14-layer decision pipeline** from input to ALLOW/DENY
- **Post-quantum safe**: ML-KEM (Kyber) + ML-DSA (Dilithium)
- **Hyperbolic geometry**: Poincaré ball model
- **995+ tests passing**

---

## The Pitch (1 Sentence)

*"We built the navigation system for AI agents - the same math that coordinates drone swarms now coordinates coding agents, so they can't drift into bugs or hallucinations."*

---

**GitHub:** [SCBE-AETHERMOORE](https://github.com/issdandavis/SCBE-AETHERMOORE)
