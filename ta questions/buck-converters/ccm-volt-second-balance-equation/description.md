# Buck converter CCM inductor volt-second balance equation

## Caption for Word image document
Buck converter CCM volt-second-balance question: during switch on-time, the inductor voltage is Vdc − Vo; during switch off-time, the freewheel diode conducts and the inductor voltage is −Vo. Volt-second balance gives δ(Vdc − Vo) − (1−δ)Vo = 0; correct option A.

## Where this belongs / folder path
`ta questions/buck-converters/ccm-volt-second-balance-equation/description.md`

## Question title / short name
Buck CCM inductor volt-second-balance equation

## Category
Buck converters

## Subcategory
CCM volt-second balance

## Key topic
Using inductor volt-second balance over one PWM period for a buck converter operating in continuous current mode.

## Full visible question text
The circuit diagram below shows a Buck converter.

The voltage and currents in the circuit can be separated into an average quantity and a ripple quantity such that `x(t) = Xbar + Δx(t)`, where `x(t)` is the signal, `Xbar` is the average and `Δx(t)` is the ripple function.

If the circuit is operated in continuous current mode with a duty ratio `δ`, the volt-seconds balance equation for `L` is given by:

Options shown:
- A: `δ(Vdc − Vo) − (1−δ)Vo = 0`
- B: `δVdc − (1−δ)Vo = 0`
- C: `δ(Vdc − Vo) − δVo = 0`
- D: `δVo − (1−δ)Vo = 0`

## Given values
- Converter: Buck converter
- Operating mode: CCM
- Duty ratio: `δ`
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Inductor: `L`

## What the question is asking for
The correct inductor volt-second balance equation for a buck converter in CCM.

## Correct answer
`A. δ(Vdc − Vo) − (1−δ)Vo = 0`

## Method summary
During Mode 1, the switch is on and the diode is off. The left side of the inductor is connected to the input supply and the right side is at the output voltage, so:

`vL,on = Vdc − Vo`

This lasts for duty fraction `δ`.

During Mode 2, the switch is off and the diode conducts. The left side of the inductor is clamped near 0 V while the output side remains at `Vo`, so:

`vL,off = −Vo`

This lasts for duty fraction `1−δ`.

Inductor volt-second balance requires zero average inductor voltage over one switching period:

`δ(Vdc − Vo) + (1−δ)(−Vo) = 0`

Therefore:

`δ(Vdc − Vo) − (1−δ)Vo = 0`

## Formula / equation source
- Formula sheet: inductor volt-second balance, `∫vL dt = 0` over one PWM period in steady state.
- Circuit reasoning: buck Mode 1 has `vL = Vdc − Vo`.
- Circuit reasoning: buck Mode 2 has `vL = −Vo`.

## Must-know concept
For a buck converter, the inductor voltage is positive during switch on-time and negative during freewheel off-time. Steady state requires the positive and negative volt-second areas to cancel.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded circuit/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a distinct converter-category question.

- Repository search found no exact existing archive entry for buck converter CCM inductor volt-second balance.
- Similar archive entries exist for boost, buck-boost, and forward converter volt-second balance, but this is stored separately because the converter topology and inductor voltage intervals are different.
- This belongs under buck converters because it is a reusable buck-specific exam theory/category question.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice question.
