# Feather & Field — Product Usefulness Plan

## Current evidence
The current known-good prototype is v0.1.1, preserved in Dropbox. It combines short active-recall A&P sessions with a small bird-sanctuary reward loop. The code has not yet been imported into this repository, so this document is a plan—not a claim that the repository contains a runnable game.

## The core question
Does the sanctuary layer help people study more consistently and remember material better, without slowing down retrieval practice or distracting from learning?

## What the first usable version must do
1. Start a study session quickly, without account creation or setup.
2. Ask clear questions with unambiguous correct answers and useful explanations.
3. Give honest feedback and track accuracy without impossible percentages.
4. Preserve progress safely across refreshes and browser restarts when storage is available.
5. Let a learner resume study and prioritize unfamiliar or weak topics.
6. Keep game rewards secondary to learning; never reward repeated guessing more than actual learning.
7. Work in a normal browser with clear messaging when saving is unavailable.

## Evaluation stages

### Stage A — Reliability (before adding features)
- Import the exact v0.1.1 package and preserve the original archive.
- Run syntax checks and the existing Node tests.
- Open the extracted app in an ordinary browser.
- Test quick session, full session, answer feedback, navigation, reward rules, adoption, and progress.
- Refresh and restart the browser to test real persistence.
- Test fresh, existing, malformed, and unavailable saved data.
- Confirm no console errors, broken assets, or horizontal overflow at phone and desktop widths.

### Stage B — Learning value
Run a small, voluntary pilot with several study sessions. Record:
- sessions started and completed
- time to first question
- questions answered per minute
- delayed accuracy on previously missed questions
- whether learners can explain missed answers after feedback
- how often the sanctuary screen interrupts or extends study
- self-reported focus, enjoyment, and frustration

Use a short baseline session without game rewards and compare it with a similar session using rewards. Avoid interpreting enjoyment or time-in-app alone as learning improvement.

### Stage C — Decide whether to keep or change gamification
Keep a game mechanic only if it improves consistency, motivation, or retention without materially reducing useful retrieval practice. Simplify or remove mechanics that add clicks, encourage grinding, obscure progress, or make rewards more important than learning.

## Feature priorities (provisional)
1. Correctness, clear explanations, robust saving, and regression tests.
2. Review scheduling that brings missed/uncertain items back at useful intervals.
3. A transparent weak-topic view and a focused "review missed questions" mode.
4. Question-bank quality controls: source, topic, difficulty, explanation, and review status.
5. Habitat discovery tied to learning milestones rather than direct bird purchases, if it proves more motivating.
6. Accessible layout, keyboard support, readable contrast, reduced motion, and responsive behavior.
7. Optional art/audio only after the core study loop is dependable.

## Guardrails
- The existing 12-question A&P bank is only a prototype, not a validated curriculum.
- Existing prices, seed amounts, and unlock thresholds are unvalidated design assumptions.
- Do not claim improved learning outcomes without actual evidence.
- Do not silently reset or migrate user saves.
- Keep a changelog, run tests after code changes, and report precisely what was tested.
