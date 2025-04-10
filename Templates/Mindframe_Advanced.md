# Mind Framework Documentation (Advanced with Optional Variables)

[OVERVIEW]
## Overview

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique. 

**Note:** Optional metadata sections such as `[PRETEXT]`, `[INSTRUCTIONS]`, and `[OUTLINERS]` are used to enhance AI interpretability and should be included only when necessary.

---

[PRETEXT] *(Optional)*
## Pretext

Lorem ipsum used to introduce the mindset, tone, or narrative lens the AI should adopt before parsing further structure.

---

[INSTRUCTIONS] *(Optional)*
## Instructions for Interpretation

Clarifies how the AI should interpret ambiguous elements or prioritize certain values.

```plaintext
- Interpret strategic ambiguity as a cue for applying highest-risk-safe assumptions.
- If multiple plausible interpretations exist, return both with ranking.
```

---

[STRUCTURE]
## Prompt Structure

[CONTEXT_LAYER]
### 1. Context Layer (Framing)

```plaintext
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus, luctus nec ullamcorper mattis, pulvinar dapibus leo.
```

---

[INSTRUCTION_LAYER]
### 2. Instruction Layer (Behavioral Guardrails)

```plaintext
- Lorem ipsum dolor sit amet.
- Consectetur adipiscing elit.
- Suspendisse varius enim in eros elementum tristique.
- Duis cursus, mi quis viverra ornare.
```

---

[INPUT_VARIABLES]
### 3. Input Variables (Modular)

```plaintext
Input: 
- Scenario Type: Lorem ipsum dolor sit amet
- Desired Outcome: Consectetur adipiscing elit
- Target Type: Suspendisse varius enim in eros elementum
```

---

[OUTPUT_FORMAT]
### 4. Output Format (Clarity Layer)

```plaintext
**Response Format:**  
1. Lorem Ipsum Summary  
2. Actionable Tactics  
3. Psychological Framing  
4. Red Flag/Warning Section
```

---

[OUTLINERS] *(Optional)*
## Edge Cases / Outliners

Used to define boundary conditions, exceptions, or how to handle highly anomalous inputs.

```plaintext
- If the target type is undefined or contradictory, return a clarification query.
- If the scenario involves legal or ethical violations, flag it and halt.
```

---

[CONDITIONS] *(Optional)*
## Conditional Logic / Context Sensitivity

```plaintext
- If tone is "cold", omit emotionally supportive language.
- If scenario mentions urgency, prioritize conciseness and speed.
```

---

[EXAMPLE_PROMPT]
## Example Prompt Usage

```plaintext
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique. 

- Lorem ipsum dolor sit amet. 
- Consectetur adipiscing elit. 
- Suspendisse varius enim in eros elementum tristique. 
- Duis cursus, mi quis viverra ornare.

Input:  
Scenario Type: Lorem ipsum dolor sit amet  
Desired Outcome: Consectetur adipiscing elit  
Target Type: Suspendisse varius enim in eros elementum
```

---

[PRESET_RESPONSES] *(Optional)*
## Preset Responses / Defaults

Used for training, calibration, or fallback.

```plaintext
If no input provided: 
Return default structure using scenario type: "interpersonal tension", outcome: "clarity"
```

---

[TEST_CONDITIONS] *(Optional)*
## Test Conditions or Format Triggers

Add sample questions or test triggers to evaluate or refine output behavior.

```plaintext
- Test: What happens if no target type is given?
- Test: Does the AI correctly detect ethical red flags?
```

---

[REPLY_FORMAT] *(Optional)*
## Final Reply Format Constraints

Use this to enforce exact formatting rules.

```plaintext
Always include:
- Bold section headers
- Bullets for all lists
- One-line summary before full breakdown
