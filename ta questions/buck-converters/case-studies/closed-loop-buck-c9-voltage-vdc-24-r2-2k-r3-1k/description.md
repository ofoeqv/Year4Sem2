# Closed-loop buck converter C9 voltage

## Caption for your Word image document
Closed-loop buck converter feedback-network case study: the circuit asks for the steady-state voltage across capacitor C9, using the feedback divider R2 = 2 kΩ and R3 = 1 kΩ with βVref = 2.5 V; in steady state, C9 is open-circuit and its voltage is set by the output voltage and feedback-node voltage.

## Where this belongs
This belongs under:

`ta questions/buck-converters/case-studies/closed-loop-buck-c9-voltage-vdc-24-r2-2k-r3-1k/`

Reason: it is a buck converter question, but specifically a closed-loop/control case-study question rather than a basic buck ripple/current-design question.

## Question title / short name
Closed-loop buck converter voltage across C9

## Category
buck converters

## Subcategory
case studies / feedback-control / capacitor-voltage

## Key topic
Steady-state voltage across a feedback-network capacitor in a closed-loop buck converter.

## Full visible question text
The diagram below shows a simplified representation of a closed-loop Buck converter power supply. Assuming the circuit is in steady-state, what is the voltage across the terminals of capacitor C9 if the circuit is operating with the following parameters:

Vdc = 24 V, R2 = 2 kΩ, R3 = 1 kΩ, βVref = 2.5 V, vsaw = 5 V

The polarity of the voltage across C9 is indicated by the direction of the arrow in the figure. Please specify your answer in units of V to 2 decimal places.

## Given values
- Input voltage, Vdc = 24 V
- R2 = 2 kΩ
- R3 = 1 kΩ
- βVref = 2.5 V
- Sawtooth amplitude, vsaw = 5 V
- Converter type: closed-loop buck converter
- Operating condition: steady state

## What the question is asking for
Find the voltage across capacitor C9, using the polarity arrow shown in the figure.

## Correct answer
VC9 = 5.00 V

## Method summary
In steady state, the feedback node is regulated to the reference level:

αVo = βVref = 2.5 V

The feedback divider ratio is:

α = R3 / (R2 + R3) = 1 / (2 + 1) = 1/3

Therefore:

Vo = 2.5 / (1/3) = 7.5 V

Capacitor C9 is in the upper feedback/feedforward branch. In steady state, capacitors are open circuits, so there is no DC current through C9 and no DC current through the series feedforward resistor branch. Therefore the lower terminal of C9 sits at the feedback-node voltage, αVo = 2.5 V, while the upper terminal sits at Vo = 7.5 V.

With the arrow polarity shown upward across C9:

VC9 = Vo − αVo = 7.5 − 2.5 = 5.0 V

So:

VC9 = 5.00 V

Cross-check with the ideal buck relation:

δ = Vo / Vdc = 7.5 / 24 = 0.3125

u = δvsaw = 0.3125 × 5 = 1.5625 V

This checks the control operating point but is not required to find VC9 directly.

## Formula / equation source
- Circuit reasoning: in steady state, capacitors behave as open circuits for DC.
- Circuit reasoning: feedback divider gives α = R3/(R2+R3).
- Closed-loop condition: αVo = βVref.
- Ideal buck relation used only as a consistency check: Vo = δVdc.
- PWM comparator relation used only as a consistency check: δ = u/vsaw.

## Must-know concept
In steady-state DC analysis, capacitors are open circuits. For C9, that means its DC voltage is set by the difference between the output rail and the feedback-divider node, not by capacitor current.

## Duplicate-check result
Not a duplicate. It is similar to the existing closed-loop buck case study, but the previous archived question asks for Vdc using vC2 = 0.5 V and different resistor labels/values. This question asks for the steady-state voltage across C9 with Vdc = 24 V, R2 = 2 kΩ and R3 = 1 kΩ.

## Date archived
2026-05-29

## Original image filename
image.png

## GitHub image storage
Image not stored in GitHub for this entry. User keeps images in a separate Word document and uses the caption above to associate the image with this archived question.

## Archive instructions applied
- Classify the question before solving.
- Check the manifest and repository search for duplicates.
- Store the question information as a markdown file on the `power-elec` branch.
- Do not store the image in GitHub; provide a caption for the separate Word image document.
- Include category, subcategory, key topic, visible question text, values, answer, method, formula/equation source, date archived, original image filename, and duplicate-check result.
