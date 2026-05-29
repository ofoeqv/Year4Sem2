# Closed-loop buck converter Vdc from C2 voltage and PWM control

## Caption for Word image document
Closed-loop buck converter feedback-control question: with R12 = 3 kΩ, R13 = 3 kΩ, βVref = 2.5 V, vsaw = 5 V, and vC2 = 0.5 V, the feedback divider gives Vo = 5.00 V and the PWM control voltage gives δ = 0.60, so the required input voltage is Vdc = 8.33 V.

## Where this belongs / folder path
`ta questions/buck-converters/case-studies/closed-loop-buck-feedback-vdc-c2-0p5v-r12-3k-r13-3k/description.md`

## Question title / short name
Closed-loop buck converter Vdc from C2 voltage, R12 = R13 = 3 kΩ

## Category
Buck converters

## Subcategory
Case studies / feedback-control / PWM duty calculation

## Key topic
Finding the required input voltage of a closed-loop buck converter from the feedback divider, op-amp/PWM control voltage, and ideal buck duty relationship.

## Full visible question text
The diagram below shows a simplified representation of a closed-loop Buck converter power supply. Assuming the circuit is in steady-state, what is the input voltage Vdc if there is a voltage of 0.5 V across C2 and the circuit is operating with the following parameters:

R12 = 3 kΩ, R13 = 3 kΩ, βVref = 2.5 V, vsaw = 5 V.

Please specify your answer in units of V to 2 decimal places.

## Given values
- Feedback resistor: `R12 = 3 kΩ`
- Feedback resistor: `R13 = 3 kΩ`
- Reference input: `βVref = 2.5 V`
- Sawtooth amplitude: `vsaw = 5 V`
- Voltage across compensation capacitor: `vC2 = 0.5 V`
- Operating condition: steady-state closed-loop buck converter

## What the question is asking for
The input voltage `Vdc` in volts.

## Correct answer
`Vdc = 8.33 V`

## Method summary
At steady state, the feedback node is regulated to the reference value:

`αVo = βVref = 2.5 V`

The feedback factor is set by the divider:

`α = R13/(R12 + R13) = 3/(3 + 3) = 0.5`

Therefore:

`Vo = 2.5/0.5 = 5.00 V`

The op-amp/PWM control voltage is increased by the voltage across `C2`:

`u = βVref + vC2 = 2.5 + 0.5 = 3.0 V`

For a sawtooth PWM comparator:

`δ = u/vsaw = 3.0/5.0 = 0.60`

For an ideal buck converter:

`Vo = δVdc`

so:

`Vdc = Vo/δ = 5.00/0.60 = 8.33 V`

## Formula / equation source
- Circuit reasoning: feedback divider `α = R13/(R12 + R13)`.
- Circuit reasoning: closed-loop steady-state condition `αVo = βVref`.
- Circuit reasoning: PWM duty ratio from comparator `δ = u/vsaw`.
- Buck converter relation from converter operation: `Vo = δVdc`.
- Formula sheet / circuit analysis support: volt-second balance underlies the ideal buck relation.

## Must-know concept
In a closed-loop buck converter, the feedback loop fixes the output voltage first. The PWM control voltage then fixes the duty ratio. Once `Vo` and `δ` are known, the required input is `Vdc = Vo/δ`.

## Date archived
2026-05-29

## Original image filename
`image.png`

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new similar-not-duplicate.

- Manifest check: a similar closed-loop buck converter question already exists asking for `Vdc` from `vC2 = 0.5 V`, but it uses `R12 = 4 kΩ` and `R13 = 3 kΩ` and has answer `9.72 V`.
- This question uses `R12 = 3 kΩ` and `R13 = 3 kΩ`, so the feedback factor and answer are different.
- Repository search: no exact repository match found for `C2 = 0.5 V`, `R12 = 3 kΩ`, `R13 = 3 kΩ`, `βVref = 2.5 V`, and `vsaw = 5 V`.
- Decision: archive as a new question.

## Uncertainty
No visible value uncertainty. The typed prompt clearly gives `R12 = 3 kΩ`, `R13 = 3 kΩ`, `βVref = 2.5 V`, `vsaw = 5 V`, and `vC2 = 0.5 V`.
