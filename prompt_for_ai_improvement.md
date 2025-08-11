# AI Prompt: Improve Planche Progression Method

## Project Context

You are helping to improve a **calisthenics workout tracking system** called "Workout Pro" - a comprehensive progression system for skill development and resistance band-assisted exercises. The system focuses on data-driven, objective progression criteria rather than subjective feel-based training.

### Project Structure
```
workout-pro/
├── README.md           # Project overview and documentation
├── BANDS.md           # Resistance bands specifications and usage
├── logs/              # Daily workout logs organized by date (YYYY/M/DD.md)
├── progress/          # Progress tracking and statistics
│   └── stats.md       # Current skills stats summary
└── skills/            # Skill-specific progression tracking
    ├── frontlever/    # Front lever progression
    ├── handstand/     # Handstand progression  
    ├── planche/       # Planche progression (THIS IS WHAT WE'RE IMPROVING)
    └── weighted-pullups/ # Weighted pull-ups progression
```

### Current Training Philosophy
- **Data-driven progression**: RPE (Rate of Perceived Exertion) scale 1-10 logged for every set
- **Objective criteria**: Clear, measurable benchmarks before advancing
- **Band-assisted training**: Using resistance bands to gradually reduce assistance
- **Machine-readable format**: YAML sections for automated tracking

## Equipment Available

**Resistance Bands Specifications:**
- Length: 100cm, Circumference: 200cm
- Available bands (5 total):
  - **6mm Yellow**: 0-3kg resistance (lightest)
  - **13mm Red**: 3-9kg resistance  
  - **22mm Black**: 9-17kg resistance (CURRENTLY USING)
  - **32mm Purple**: 17-22kg resistance
  - **44mm Green**: 22-32kg resistance (heaviest available)

## Current Planche Status (80kg athlete)

**Current Level**: Early-intermediate (Advanced-tuck → Straddle transition)
**Current Band**: 22mm Black (9-17kg assistance)
**Target Band**: 13mm Red (3-9kg assistance)

### Recent Performance Data (Last 4 Sessions)
```
2025-07-15: 11s, 10s, 9s, 10s @RPE 8 (Advanced-tuck, Black band)
2025-07-18: 8s, 11s, 9s, 10s @RPE 8 (Advanced-tuck, Black band)  
2025-07-21: 10s, 8s, 10s, 12s @RPE 8 (Advanced-tuck, Black band)
2025-07-22: 8s, 8s, 11s, 9s, 11s @RPE 8 (Advanced-tuck, Black band)
```

**Straddle Attempts (higher difficulty):**
```
2025-07-17: 1s, 1s, 2s, 2s, 3s, 4s @RPE 9 (Straddle, Black+Red bands)
2025-07-21: 3s, 4s, 4s @RPE 8-9 (Straddle, Black+Red bands)
```

**Current Challenge**: Athlete has been stuck at RPE 8 for 4 consecutive sessions. Progression criteria require RPE ≤7 for 2 consecutive sessions before advancing to red band.

## Task: Improve the Planche Progression File

**Your goal**: Analyze the current planche progression methodology and create an improved version that addresses the following issues:

### Problems to Address:
1. **RPE Plateau**: Athlete stuck at RPE 8, not progressing to RPE 7
2. **Lack of Intermediate Steps**: Current system only has major band drops (22mm→13mm)
3. **Missing Troubleshooting**: No guidance for RPE plateaus
4. **Volume/Intensity Balance**: May need periodization or deload protocols
5. **Straddle Integration**: How to properly integrate straddle practice with advanced-tuck training
6. **Recovery Protocols**: Limited guidance on managing fatigue/adaptation

### Current Progression File Content:

```markdown
# Planche Band‑Assisted Progression Method

> **Scope:** Advanced‑tuck → Straddle → Full planche using long loop bands (22 mm ▶︎ 13 mm ▶︎ 6 mm).  This file defines the objective rules the AI should follow when deciding whether a band/shape progression has been earned.

---

## 1  Key Variables That Drive the Timeline

| Variable               | Speeds progression                                 | Slows progression                          |
| ---------------------- | -------------------------------------------------- | ------------------------------------------ |
| **Training frequency** | 3 focused sessions / week                          | 1–2 sessions / week                        |
| **Recovery habits**    | 7–9 h sleep, 1.6–2 g protein / kg, low life‑stress | Poor sleep, low protein, frequent max‑outs |
| **Starting buffer**    | Already at **4 × 10–12 s**, `RPE ≤ 7`              | Only 1–2 sets ≥ 8 s, `RPE 9–10`            |
| **Body‑weight change** | Losing a few kg (less load)                        | Gaining mass (more load)                   |

---

## 2  Data‑Driven Progression Rule  📏

> **Progress ONLY when:**
>
> * You can perform **4 – 5 work sets** of **8–12 s** each **AND**
> * The **last set RPE ≤ 7**, **for two consecutive sessions**.

If either condition is not met, **repeat** the same band/shape next session.

### Session Assumptions

* 2–3 planche sessions per week
* Rest 90–120 s between work sets
* RPE logged immediately after every set (whole‑number scale 1–10)

---

## 3  Typical Ranges per Athlete Tier

| Athlete tier                                 | Sessions per band drop | Weeks (at 2‑3×/wk) |
| -------------------------------------------- | ---------------------- | ------------------ |
| **Beginner** (tuck)                          | 6 – 9                  | ≈ 3 – 5            |
| **Early‑intermediate** (adv‑tuck → straddle) | 8 – 12                 | ≈ 4 – 6            |
| **Late‑intermediate** (straddle → full)      | 10 – 15                | ≈ 5 – 8            |
| **Advanced** (< 13 mm or no band)            | 12 – 18                | ≈ 6 – 10           |

> **Current status:** `early-intermediate` → expect **8–12 quality sessions** (≈ 4–6 wk @ 2×/wk) to move from **black 22 mm** to **red 13 mm** if criteria are met.

---

## 4  Refining the Estimate for *You*

1. **Baseline test:** `4 × 10 s` advanced‑tuck with black 22 mm; log every RPE.

2. **Project the drop‑curve:**

   | Session | Avg RPE                    |
   | ------- | -------------------------- |
   | 1–2     | 9                          |
   | 3–4     | 8                          |
   | 5–6     | 7 → **progression earned** |

3. **Adjust on the fly:**

   * If RPE barely moves → add rest days or volume‑neutral deload.
   * If RPE plunges quickly → progression may come in 4–5 sessions.

---

## 5  Self‑Check Template (add to every log)

```text
Did I finish all sets?  Y/N
Last‑set RPE: ___
If RPE ≤ 7 **two sessions in a row**, progress next time.
```

---

## 6  Practical Timeline Example  (80 kg, **black 22 mm → red 13 mm**)

| Week | Mon                              | Thu                                             |
| ---- | -------------------------------- | ----------------------------------------------- |
| 1    | 4 × 10 s @ RPE 9                 | 4 × 10 s @ RPE 8.5                              |
| 2    | 4 × 12 s @ RPE 8                 | 5 × 10 s @ RPE 7.5                              |
| 3    | 4 × 12 s @ RPE 7 ✓ (second time) | **Switch to red band** → expect 4 × 8 s @ RPE 9 |

Total: **5 sessions → \~2.5 weeks** (may stretch to 4–5 wk if recovery lags).

---

## 7  Machine‑Readable Summary <!-- for downstream scripts -->

```yaml
progression_criteria:
  sets: 4-5
  hold_seconds: 8-12
  last_set_rpe_max: 7
  consecutive_sessions: 2
band_drop_estimates:
  beginner:       { sessions: 6-9,  weeks: 3-5 }
  early_intermediate: { sessions: 8-12, weeks: 4-6 }
  late_intermediate:  { sessions: 10-15, weeks: 5-8 }
  advanced:       { sessions: 12-18, weeks: 6-10 }
current_status:
  tier: early_intermediate
  current_band: 22mm
  target_band: 13mm
```

---

### 📌 Bottom Line

1. **Track**: sets, seconds, RPE every session.
2. **Meet criteria** twice consecutively → drop band **or** upgrade shape (never both).
3. **Typical pace:** 22 mm → 13 mm inside \~ 1 month at 2–3 sessions per week.
4. **Let numbers—not the calendar—drive the call.**
```

## Requirements for Improvement

### Must Include:
1. **RPE Plateau Solutions**: Specific protocols when stuck at same RPE for 3+ sessions
2. **Intermediate Progression Steps**: Smaller progressions between major band changes
3. **Periodization Framework**: Deload weeks, volume cycling, intensity management
4. **Troubleshooting Section**: Common sticking points and solutions
5. **Advanced Integration**: How to incorporate straddle/full planche practice
6. **Recovery Protocols**: Active recovery, fatigue management, adaptation phases
7. **Form Diagnostics**: Technical breakdowns affecting progression
8. **Band Combinations**: Using multiple bands or partial assistance methods

### Maintain:
- **Machine-readable YAML sections** for automated tracking
- **Data-driven approach** with objective criteria
- **RPE-based progression** system
- **Conservative progression** philosophy (safety first)
- **Current structure** (7 sections + machine-readable summary)

### Output Format:
Please provide a complete, improved `progression.md` file that directly replaces the current one, incorporating all the improvements while maintaining compatibility with the existing tracking system.

The improved file should help this specific athlete break through their current RPE plateau and provide more nuanced progression pathways.