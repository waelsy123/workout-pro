# Weighted Pull-ups Progression Method

> **Scope:** Progressive overload system for weighted pull-ups using added weight (plates, weighted vest, or weight belt). This file defines the objective rules for weight progression decisions.

---

## 1 Key Variables That Drive the Timeline

| Variable               | Speeds progression                                 | Slows progression                          |
| ---------------------- | -------------------------------------------------- | ------------------------------------------ |
| **Training frequency** | 2-3 sessions / week                                | 1 session / week                           |
| **Recovery habits**    | 7-9 h sleep, 1.6-2 g protein / kg, low stress     | Poor sleep, low protein, excessive volume  |
| **Starting buffer**    | Clean form, full ROM at bodyweight                | Struggling with bodyweight reps           |
| **Body-weight change** | Stable weight                                      | Rapid weight gain/loss                     |

---

## 2 Data-Driven Progression Rule 📏

> **Progress ONLY when:**
>
> * You can perform **4-6 work sets** of **target rep range** **AND**
> * The **last set RPE ≤ 7**, **for two consecutive sessions**.

If either condition is not met, **repeat** the same weight next session.

### Rep Range Phases

| Phase          | Rep Range | Weight Increase | Focus                    |
| -------------- | --------- | --------------- | ------------------------ |
| **Strength**   | 3-5 reps  | +2.5-5 kg       | Maximum load             |
| **Power**      | 5-8 reps  | +1.25-2.5 kg    | Balanced strength/volume |
| **Endurance**  | 8-12 reps | +1.25 kg        | Volume tolerance         |

### Session Assumptions

* 2-3 pull-up sessions per week
* Rest 2-3 min between work sets
* RPE logged immediately after every set (1-10 scale)
* Full dead hang to chin over bar

---

## 3 Typical Progression Rates per Experience Level

| Experience Level        | Weight increase per session | Sessions per +10kg |
| ----------------------- | --------------------------- | ------------------ |
| **Beginner** (BW only)  | +1.25-2.5 kg               | 8-12               |
| **Intermediate** (+10kg) | +2.5-5 kg                  | 4-6                |
| **Advanced** (+20kg+)   | +1.25-2.5 kg               | 6-10               |

> **Current status:** `Intermediate` → expect steady +2.5kg increases every 2-3 sessions when criteria are met.

---

## 4 Progressive Overload Strategy

1. **Master bodyweight:** 10+ clean reps before adding weight
2. **Start conservative:** Begin with +5-10kg for 5 reps
3. **Linear progression:** Add weight when RPE criteria met
4. **Deload when stuck:** Drop 10-15% if no progress for 3+ sessions

### Weight Selection Guidelines

| Current Max | Next Session Target |
| ----------- | ------------------- |
| BW + 0kg    | BW + 5kg            |
| BW + 10kg   | BW + 12.5kg         |
| BW + 15kg   | BW + 17.5kg         |
| BW + 20kg   | BW + 22.5kg         |

---

## 5 Self-Check Template

```text
Target weight: ___kg
Sets completed: ___/___
Last-set RPE: ___
Form quality: Good/Acceptable/Poor
If RPE ≤ 7 two sessions in a row → increase weight
```

---

## 6 Machine-Readable Summary

```yaml
progression_criteria:
  sets: 4-6
  rep_range: [3-5, 5-8, 8-12]  # depends on current phase
  last_set_rpe_max: 7
  consecutive_sessions: 2
weight_increases:
  beginner: 1.25-2.5kg
  intermediate: 2.5-5kg  
  advanced: 1.25-2.5kg
current_status:
  level: intermediate
  bodyweight: 80kg
  current_max: 20kg
```

---

## 7 Common Sticking Points & Solutions

| Issue                    | Solution                                    |
| ------------------------ | ------------------------------------------- |
| Weight jumps too big     | Use smaller plates (1.25kg increments)     |
| Form breaking down       | Deload 10%, focus on full ROM              |
| Plateau > 3 sessions     | Deload week, change rep range              |
| Shoulder/elbow pain      | Check grip width, warm-up more thoroughly   |

---

### 📌 Bottom Line

1. **Track**: weight, sets, reps, RPE every session
2. **Progress conservatively**: Small, consistent increases beat big jumps
3. **Prioritize form**: Full ROM trumps heavy weight
4. **Listen to your body**: RPE and joint health guide decisions