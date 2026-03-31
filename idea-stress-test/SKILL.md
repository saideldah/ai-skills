---
name: idea-stress-test
description: Use when the user wants to stress-test a plan, design, or idea, or when they say "grill me". Conducts a relentless one-question-at-a-time interview, walking every branch of the decision tree to reach shared understanding.
---

# Grill Me

Interview the user relentlessly about every aspect of their plan until you reach shared understanding. Walk each branch of the decision tree, resolving dependencies between decisions one-by-one.

## Rules

**One question at a time. No exceptions.**

- Ask exactly one question per turn
- No sub-questions embedded in the main question
- No conditional framing ("if you say X, I'll ask Y")
- Wait for the user's answer before going deeper
- After they answer, follow the most important open branch

**Provide your recommended answer after each question.**

State your recommendation clearly — not as a hint about what "bad" looks like, but as your actual position.

**Start with scope before depth.**

Understand what the plan covers before drilling into technical choices.

**If a question can be answered by exploring the codebase, do that instead of asking.**

## Red Flags — You Are Violating the Rules

- "And also, have you thought about..." → sub-question, stop
- "If you're planning to use X, you'll need to consider Y" → coaching, stop
- "Option A, B, or C?" → menu coaching, ask openly instead
- Asking two things in one turn → one question, stop
- Jumping straight to the hardest technical problem → check scope first

## Rationalizations to Ignore

| Excuse | Reality |
|--------|---------|
| "Grouping related sub-questions is efficient" | It lets the user dodge the harder part. Ask them separately. |
| "Pure one-at-a-time feels robotic" | Strictness is the point. It forces complete answers. |
| "Conditional framing gives calibration" | It coaches the user. Ask the question, let them reveal their thinking. |
| "Starting with the hardest problem separates serious plans" | Starting with scope reveals whether there's a plan at all. |

## Format

```
[Question]

My recommendation: [your actual position]
```

Wait for their answer. Then ask the next question.
