# Boost converter CCM inductor volt-second balance equation

## Caption for Word image document
Boost converter CCM volt-second-balance question: during switch on-time, the inductor voltage is Vdc; during switch off-time, the inductor voltage is Vdc − Vo. Volt-second balance gives δVdc + (1−δ)(Vdc − Vo) = 0; correct option A.

## Where this belongs / folder path
`ta questions/Boost convertes/boost-ccm-volt-second-balance-equation/description.md`

## Question title / short name
Boost CCM inductor volt-second-balance equation

## Category
Boost convertes

## Subcategory
CCM volt-second balance

## Key topic
Using inductor volt-second balance over one PWM period for a boost converter operating in continuous current mode.

## Full visible question text
The circuit diagram below shows a Boost converter.

The voltage and currents in the circuit can be separated into an average quantity and a ripple quantity such that `x(t) = Xbar + Δx(t)`, where `x(t)` is the signal, `Xbar` is the average and `Δx(t)` is the ripple function.

If the circuit is operated in continuous current mode with a duty ratio δ, the volt-seconds balance equation for L is given by:

Options shown:
- A: `δVdc + (1−δ)(Vdc − Vo) = 0`
- B: `(1−δ)Vdc + (1−δ)(Vdc − Vo) = 0`
- C: `δVdc + (1−δ)Vo = 0`
- D: `δVdc + (1−δ)(Vdc + Vo) = 0`

## Given values
- Converter: Boost converter
- Operating mode: CCM
- Duty ratio: `δ`
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Inductor: `L`

## What the question is asking for
The correct inductor volt-second balance equation for a boost converter in CCM.

## Correct answer
`A. δVdc + (1−δ)(Vdc − Vo) = 0`

## Method summary
During Mode 1, the switch is on and the diode is off. The inductor is charged directly from the input supply, so:

`vL = Vdc`

This lasts for duty fraction `δ`.

During Mode 2, the switch is off and the diode is on. The inductor is connected between the input and the output, so:

`vL = Vdc − Vo`

This lasts for duty fraction `1−δ`.

Inductor volt-second balance requires the average inductor voltage over one switching period to be zero:

`δVdc + (1−δ)(Vdc − Vo) = 0`

## Formula / equation source
- Formula sheet: inductor volt-second balance, `∫vL dt = 0` over one PWM period in steady state.
- Circuit reasoning: boost Mode 1 has switch on and diode off, so `vL = Vdc`.
- Circuit reasoning: boost Mode 2 has switch off and diode on, so `vL = Vdc − Vo`.

## Must-know concept
For a boost converter, the inductor charges from the input during switch-on and discharges into the output during switch-off. Since `Vo > Vdc`, the off-time inductor voltage `Vdc − Vo` is negative.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded circuit/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as distinct category question.

- Earlier check flagged this as duplicate-logic candidate relative to volt-second-balance equation questions.
- User clarified these should be stored because buck and boost charge/volt-second balance questions form distinct converter-category question types.
- Repository search found no exact existing archive entry for boost converter CCM volt-second-balance equation.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice question rather than a numerical calculation.
