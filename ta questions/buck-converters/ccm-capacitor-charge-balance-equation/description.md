# Buck converter CCM capacitor charge-balance equation

## Caption for Word image document
Buck converter CCM charge-balance question: because the output capacitor current is the difference between the inductor current and the load current in both switch intervals, charge balance gives δ(IL − Io) + (1−δ)(IL − Io) = 0; correct option B.

## Where this belongs / folder path
`ta questions/buck-converters/ccm-capacitor-charge-balance-equation/description.md`

## Question title / short name
Buck CCM capacitor charge-balance equation

## Category
Buck converters

## Subcategory
CCM charge balance

## Key topic
Using capacitor charge balance over one PWM period for a buck converter operating in continuous current mode.

## Full visible question text
The circuit diagram below shows a Buck converter.

The voltage and currents in the circuit can be separated into an average quantity and a ripple quantity such that `x(t) = Xbar + Δx(t)`, where `x(t)` is the signal, `Xbar` is the average and `Δx(t)` is the ripple function.

If the circuit is operated in continuous current mode with a duty ratio δ, the charge balance equation for C is given by:

Options shown:
- A: `δ(IL − Io) − (1−δ)(IL − Io) = 0`
- B: `δ(IL − Io) + (1−δ)(IL − Io) = 0`
- C: `δ(IL − Io) − (1−δ)IL = 0`
- D: `δIL − (1−δ)(IL − Io) = 0`

## Given values
- Converter: Buck converter
- Operating mode: CCM
- Duty ratio: `δ`
- Average inductor current: `IL`
- Average output current: `Io`
- Output capacitor: `C`

## What the question is asking for
The correct capacitor charge-balance equation for a buck converter in CCM.

## Correct answer
`B. δ(IL − Io) + (1−δ)(IL − Io) = 0`

## Method summary
In a buck converter, the capacitor is connected at the output node in both switching intervals. Therefore the capacitor current is the difference between the inductor current and the load current:

`iC = iL − Io`

This is true during both the switch-on and switch-off intervals. Over one full switching period, capacitor charge balance requires average capacitor current to be zero:

`δ(IL − Io) + (1−δ)(IL − Io) = 0`

Since `δ + (1−δ) = 1`, this also implies:

`IL − Io = 0`

so in steady state:

`IL = Io`

## Formula / equation source
- Formula sheet: capacitor charge balance, `∫ iC dt = 0` over one PWM period in steady state.
- Circuit reasoning: for the buck output node, `iC = iL − Io` in both ON and OFF intervals.

## Must-know concept
For a buck converter in CCM, the average inductor current equals the average load current because the capacitor cannot absorb or deliver net charge over a full switching period.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded circuit/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as distinct category question.

- Earlier check flagged this as duplicate-logic candidate relative to charge-balance equation questions.
- User clarified these should be stored because buck and boost charge/volt-second balance questions form distinct converter-category question types.
- Repository search found no exact existing archive entry for buck converter CCM capacitor charge-balance equation.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice question rather than a numerical calculation.
