# Cognitive Lifecycle — System Contract v1.1

## 🔄 Pipeline
`React` → `Perceive` → `Feel` → `Interpret` → `Decide` → `Express` → `Remember`
*(Global feedback + asynchronous timing)*

---

## 🛠 Core Properties (System-Wide)
- **Temporal persistence** across cycles
- **Parallel hypothesis** tracking
- **Constraint-based** rejection
- **Lossy compression** at every boundary
- **Emotional weighting** of compute + memory
- **Causal simulation** over correlation
- **Finite memory capacity** + mandatory forgetting
- **Continuous feedback** between stages

---

## 📑 Stage Contracts

### ⚡ React
- **Produces:** arousal scalar, valence polarity, priority weight
- **Properties:** persistent background state, fastest stage, biases all downstream, non-semantic.

### 🔍 Perceive
- **Produces:** segmented units, ambiguity score, contextual markers
- **Properties:** lossy but revisable, multi-segmentation active, discrete hypothesis set.

### 💓 Feel
- **Produces:** emotion label(s), intensity, decay constant
- **Properties:** momentum across cycles, modulates memory encoding, biases interpretation.

### 🧠 Interpret
- **Produces:** causal models, intent hypotheses, expectations, narrative fits
- **Properties:** multiple parallel models, constraint-checked, simulation-based, socially grounded.

### ⚖️ Decide
- **Produces:** committed action, rejected options, risk estimate
- **Properties:** single collapse point, goal-conditioned, time-variable, cost-aware.

### 🗣 Express
- **Produces:** utterance / action, tone modulation, social filter output
- **Properties:** lossy compression, irreversible, emotion-shaped, channel-limited.

### 💾 Remember
- **Writes:** event narrative, emotional weight, contextual anchors, relationship deltas
- **Properties:** consolidation over time, distortion allowed, retention-weighted, forgetting mandatory.

---

## 📈 Feedback Loops
- **React** persists into next cycle.
- **Feel** & **Remember** bias **Interpret**.
- **Express** feeds **Remember**.
- **Decide** influences future goals.

---

## ⏱ Temporal Ordering (Approximate)
| Stage | Latency |
| :--- | :--- |
| **React** | 10–50 ms |
| **Perceive** | 50–100 ms |
| **Feel** | 100–500 ms |
| **Interpret** | 200 ms – 5 s |
| **Decide** | Variable |
| **Express** | ~500 ms |
| **Remember** | Background / Offline |

---

## 📌 Invariants
- `Interpret` maintains competing hypotheses; `Decide` collapses to one.
- `Express` never expands state (compression only).
- `Remember` stores interpretations, not raw signals.
- Emotional intensity increases retention.
- Impossible causal models are rejected.
