# Closed-loop buck converter input voltage from feedback control

## Caption for your Word image document
Closed-loop buck converter feedback-control case study: the circuit uses a PWM sawtooth comparator, compensator output, and feedback divider to determine the required input voltage Vdc when vC2 = 0.5 V, R12 = 4 kΩ, R13 = 3 kΩ, βVref = 2.5 V, and vsaw = 5 V.

## Question title / short name
Closed-loop buck converter Vdc from C2 voltage and PWM control

## Category
buck converters

## Subcategory
case studies / feedback-control

## Key topic
Closed-loop buck converter steady-state control calculation.

## Full visible question text
Question 3

The diagram below shows a simplified representation of a closed-loop Buck converter power supply. Assuming the circuit is in steady-state, what is the input voltage Vdc if there is a voltage of 0.5 V across C2 and the circuit is operating with the following parameters:

R12 = 4 kΩ, R13 = 3 kΩ, βVref = 2.5 V, vsaw = 5 V

Please specify your answer in units of V to 2 decimal places.

## Given values
- R12 = 4 kΩ
- R13 = 3 kΩ
- βVref = 2.5 V
- vsaw = 5 V
- Voltage across C2 = 0.5 V
- Converter type: closed-loop buck converter
- Operating condition: steady state

## What the question is asking for
Find the required DC input voltage Vdc.

## Correct answer
Vdc = 9.72 V

## Method summary
In steady state, the feedback node equals the reference level:

αVo = βVref = 2.5 V

The feedback divider ratio is:

α = R13 / (R12 + R13) = 3 / (4 + 3) = 3/7

So the output voltage is:

Vo = 2.5 / (3/7) = 5.833 V

The C2 voltage gives the PWM control voltage:

u = αVo + vC2 = 2.5 + 0.5 = 3.0 V

The PWM duty ratio is:

δ = u / vsaw = 3.0 / 5.0 = 0.6

For an ideal buck converter in CCM / steady state:

Vo = δVdc

Therefore:

Vdc = Vo / δ = 5.833 / 0.6 = 9.72 V

## Formula / equation source
- Formula-sheet / standard converter relation: ideal buck converter voltage relation, Vo = δVdc.
- Circuit reasoning: feedback divider gives α = R13 / (R12 + R13).
- Circuit reasoning: in closed-loop steady state, the feedback signal is regulated to the reference level, so αVo = βVref.
- PWM reasoning: duty ratio is set by comparator relation δ = u / vsaw.

## Must-know concept
In a closed-loop buck converter, the control circuit chooses the duty ratio needed to make the feedback voltage match the reference. Once duty is known, the ideal buck relation Vo = δVdc links output voltage to input voltage.

## Date archived
2026-05-29

## Original image filename
image.png

## GitHub image storage
Image not stored in GitHub for this entry. User will keep the image in a separate Word document and use the caption above to associate the image with this archived question.

## Duplicate-check result
New question. No duplicate was found in the existing manifest, and repository search found no matching stored question/values before archiving.
