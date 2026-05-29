# Closed-loop buck converter beta from feedback bias current

## Caption for Word image document
Closed-loop buck converter feedback-divider question: with bias current through R12 of 1 mA, R13 = 3 kΩ, and Vref = 7.79 V, the feedback node voltage is 3.00 V, so the required reference scaling factor is β = 0.39.

## Where this belongs / folder path
`ta questions/buck-converters/case-studies/closed-loop-buck-feedback-beta-bias-current-r12-1ma-r13-3k-vref-7p79/description.md`

## Question title / short name
Closed-loop buck converter beta from feedback bias current

## Category
Buck converters

## Subcategory
Case studies / feedback-control / reference-scaling factor

## Key topic
Finding the required reference scaling factor `β` from the feedback-divider current and reference voltage.

## Full visible question text
The diagram below shows a simplified representation of a closed-loop Buck converter power supply. Assuming the circuit is in steady-state, what value for β is required if the bias current through R12 IBIAS = 1 mA, R13 = 3 kΩ and the reference voltage Vref = 7.79 V?

## Given values
- Bias current through `R12`: `IBIAS = 1 mA`
- Lower feedback resistor: `R13 = 3 kΩ`
- Reference voltage: `Vref = 7.79 V`
- Operating condition: steady-state closed-loop buck converter

## What the question is asking for
The required reference scaling factor `β`.

## Correct answer
`β = 0.39`

## Method summary
In steady state, the op-amp inputs are balanced, so the feedback voltage equals the scaled reference:

`αVo = βVref`

The given bias current through the feedback divider also flows through `R13` under the usual divider-current assumption, so the feedback node voltage is:

`αVo = IBIAS × R13`

Substitute the values:

`αVo = 1 mA × 3 kΩ = 3.00 V`

Then:

`β = αVo / Vref = 3.00 / 7.79 = 0.3851 ≈ 0.39`

## Formula / equation source
- Circuit reasoning: in steady-state closed-loop operation, the op-amp inputs are equal, so `αVo = βVref`.
- Circuit reasoning / Ohm's law: the feedback node voltage across `R13` is `IBIAS × R13`.
- Derived equation: `β = IBIAS R13 / Vref`.

## Must-know concept
In the feedback divider, the voltage at the feedback node is the voltage across the lower resistor `R13`. In steady state the control loop forces that feedback-node voltage to match the scaled reference `βVref`.

## Date archived
2026-05-29

## Original image filename
`image.png`

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic.

- Manifest check: existing closed-loop buck feedback entries ask for `Vdc` from `C2` voltage/PWM duty or for voltage across `C9`; they use the same circuit family but ask for different elements and use different solving tools.
- Duplicate-logic check: not flagged as duplicate logic because this question asks for `β` using `IBIAS`, `R13`, and `Vref`, rather than asking for `Vdc`, `C9`, duty ratio, or output voltage.
- Repository search: no exact repository match found for `β`, `IBIAS = 1 mA`, `R13 = 3 kΩ`, and `Vref = 7.79 V`.

## Uncertainty
No visible value uncertainty. The typed prompt clearly gives `IBIAS = 1 mA`, `R13 = 3 kΩ`, and `Vref = 7.79 V`. The solution assumes the feedback divider current through `R12` is the same current through `R13`, with negligible op-amp input current.
