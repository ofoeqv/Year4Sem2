# Buck-boost converter CCM capacitor charge-balance equation

## Caption for Word image document
Buck-boost converter CCM charge-balance question: during switch on-time the diode is off and the output capacitor supplies the load, so iC = −Io; during switch off-time the inductor current flows to the output and iC = IL − Io. Charge balance gives −δIo + (1−δ)(IL − Io) = 0; correct option A.

## Where this belongs / folder path
`ta questions/buck-boost-converter/ccm-capacitor-charge-balance-equation/description.md`

## Question title / short name
Buck-boost CCM capacitor charge-balance equation

## Category
Buck-boost converter

## Subcategory
CCM charge balance

## Key topic
Using capacitor charge balance over one PWM period for an inverting buck-boost converter operating in continuous current mode.

## Full visible question text
The circuit diagram below shows a Buck-Boost converter.

The voltage and currents in the circuit can be separated into an average quantity and a ripple quantity such that `x(t) = Xbar + Δx(t)`, where `x(t)` is the signal, `Xbar` is the average and `Δx(t)` is the ripple function.

If the circuit is operated in continuous current mode with a duty ratio `δ`, the charge balance equation for `C` is given by:

Options shown:
- A: `−δIo + (1−δ)(IL − Io) = 0`
- B: `δIo + (1−δ)(IL − Io) = 0`
- C: `−δ(IL − Io) + (1−δ)(IL − Io) = 0`
- D: `δIo + (1−δ)(IL − Io) = 0`

## Given values
- Converter: Buck-Boost converter
- Operating mode: CCM
- Duty ratio: `δ`
- Average inductor current: `IL`
- Average output/load current: `Io`
- Output capacitor: `C`

## What the question is asking for
The correct capacitor charge-balance equation for a buck-boost converter in CCM.

## Correct answer
`A. −δIo + (1−δ)(IL − Io) = 0`

## Method summary
During Mode 1, the switch is on and the diode is off. The inductor is charged from the input and the output capacitor alone supplies the load, so:

`iC = −Io`

This lasts for duty fraction `δ`.

During Mode 2, the switch is off and the diode is on. The inductor releases energy to the output. The capacitor current is the inductor/output-side current remaining after the load current is supplied:

`iC = IL − Io`

This lasts for duty fraction `1−δ`.

Capacitor charge balance requires zero average capacitor current over one full switching period:

`δ(−Io) + (1−δ)(IL − Io) = 0`

Therefore:

`−δIo + (1−δ)(IL − Io) = 0`

This also rearranges to:

`(1−δ)IL = Io`

which is the expected average-current relation for the inverting buck-boost converter.

## Formula / equation source
- Formula sheet: capacitor charge balance, `∫iC dt = 0` over one PWM period in steady state.
- Circuit reasoning: during switch on-time, the diode is off, so the capacitor supplies the load.
- Circuit reasoning: during switch off-time, the diode conducts and the inductor supplies the output.

## Must-know concept
For boost and buck-boost output stages, the output capacitor supplies the load during switch on-time. During switch off-time, the inductor feeds the output, so capacitor current becomes the difference between inductor-side output current and load current.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded circuit/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a distinct converter-category question.

- Repository search found no exact existing archive entry for buck-boost converter CCM capacitor charge balance.
- Similar archive entries exist for boost CCM capacitor charge balance and buck CCM capacitor charge balance, but this is stored separately because the converter topology and revision category are distinct.
- The method uses the same broad capacitor charge-balance principle, but the question belongs under the buck-boost converter category.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice question. Options B and D appear visually similar or identical in the screenshot, but the correct expression is option A.
