# LLM Failure Point Analysis

> **Core Thesis:** LLMs are statistical compression of human discourse without access to the four orthogonal axes required for intelligence.

---

## 🧭 The Four Axes of Grounding

| Axis | Grounds | Question | LLM Status |
|:-----|:--------|:---------|:-----------|
| **Temporal** | WHEN | Does state persist across time? | ❌ Stateless |
| **Referential** | WHAT / WHERE | Is there connection to world? | ❌ Ungrounded |
| **Evaluative** | WHY | Does anything matter to the system? | ❌ No valence |
| **Reflexive** | WHO | Does the system model itself? | ❌ No self |

---

## ⏱️ Temporal Axis — *The When*

> **Constraint:** No persistent state (resets each call)

Without temporal grounding, the system cannot:
- Maintain continuity across interactions
- Track goals over time
- Accumulate experience into trajectory
- Know "now" vs "then"

### Failures Generated

| Failure | Description |
|:--------|:------------|
| Statelessness | Complete reset between inferences |
| Context drift | Loses conversation direction over turns |
| Context limits | Hard window size constraints |
| Lost-in-middle | Poor retention of mid-context information |
| Instruction drift | Loses original goal over long generation |
| Knowledge cutoff | Static training data, no real-time awareness |
| No affect | Cannot carry emotional state forward |

---

## 🌍 Referential Axis — *The What/Where*

> **Constraint:** No world grounding (only has text)

Without referential grounding, the system cannot:
- Connect symbols to real-world referents
- Distinguish correlation from causation
- Model physical or causal relationships
- Verify claims against reality

### Failures Generated

| Failure | Description |
|:--------|:------------|
| Hallucinations | Confident fabrication of non-existent facts |
| Symbol grounding problem | No connection between words and referents |
| Causal reasoning failure | Correlation masquerading as causation |
| Counting failures | Cannot reliably count objects or tokens |
| Quantitative reasoning | Can't compare magnitudes reliably |
| Embodied understanding | No physical world model or sensorimotor experience |
| Binding problem | Struggles processing multiple distinct objects simultaneously |
| Tokenization artifacts | Signal destruction at input layer |

---

## ⚖️ Evaluative Axis — *The Why*

> **Constraint:** No valence, no preference, no stakes

Without evaluative grounding, the system cannot:
- Prioritize one thought over another
- Know when to stop or backtrack
- Feel cost of errors
- Collapse possibility space into committed action

### Failures Generated

| Failure | Description |
|:--------|:------------|
| No agency | Pure input→output, no goal-directed behavior |
| Sycophancy | Agrees rather than corrects (no cost to being wrong) |
| Verbosity | Optimizes for plausible length over clarity |
| Planning myopia | No true multi-step lookahead (nothing at stake) |
| Uncertainty failure | Makes up answers rather than admitting "I don't know" |
| Overconfidence | No felt cost for being wrong |
| Repetition loops | Gets stuck in patterns (no pain signal to escape) |

---

## 🪞 Reflexive Axis — *The Who*

> **Constraint:** No self-model, no introspection

Without reflexive grounding, the system cannot:
- Model its own behavior across time
- Predict its own responses
- Detect its own errors mid-generation
- Maintain identity or trajectory

### Failures Generated

| Failure | Description |
|:--------|:------------|
| No metacognition | Can't assess own reasoning quality |
| Self-contradiction | No verification mid-generation |
| Theory of Mind failures | Can't reliably model perspectives (including own) |
| Reversal curse | If trained "A is B", doesn't know "B is A" |
| Einstellung effect | Fixation on patterns, can't recognize own rigidity |
| Non-determinism | Different outputs for identical inputs (no self-consistency) |
| No self-correction | Cannot recognize when approach is failing |

---

## 🔀 Cross-Axis Failures

Some failures emerge from the intersection of missing axes:

| Failure | Missing Axes | Mechanism |
|:--------|:-------------|:----------|
| Prompt injection | Referential + Evaluative | Can't distinguish instruction from data, no stakes for compliance |
| Anchoring bias | Temporal + Reflexive | Early context dominates, can't observe own bias |
| Framing effects | Referential + Reflexive | No stable world model or self-model to anchor against |
| Social biases | Referential + Evaluative | Reflects training data, no cost for prejudice |
| Coordination failures | Temporal + Evaluative | Can't maintain joint objectives without persistence + stakes |

---

## 📊 Signal Loss Estimates

| Axis | Approximate Signal Retained |
|:-----|:----------------------------|
| Referential | ~15% (tokenization destroys grounding) |
| Temporal | ~0% (complete reset each call) |
| Evaluative | ~5% (RLHF approximates, doesn't instantiate) |
| Reflexive | ~10% (implicit self-model in weights, not accessible) |

---

## 🎯 Implications for API Architecture

Each axis maps to architectural requirements:

| Axis | Required Component |
|:-----|:-------------------|
| Temporal | Canonical Log, Remember stage, persistent state |
| Referential | World Model, embodiment, causal grounding |
| Evaluative | Pain Neuron, Spirit, Valuation primitive |
| Reflexive | Self-Model, Self-Observation, Soul |

> **The Core Claim:** An LLM with all four axes grounded is no longer "just" an LLM—it becomes a substrate for intelligence rather than a simulation of discourse.

---

## 📎 Summary

```
LLM = f(input) → output

API = f(input, temporal_state, world_model, valuation, self_model) → output + state_updates
```

The transformation from **frozen function** to **living architecture** requires grounding all four axes simultaneously. Partial grounding produces partial capabilities; full grounding produces the preconditions for agency.
