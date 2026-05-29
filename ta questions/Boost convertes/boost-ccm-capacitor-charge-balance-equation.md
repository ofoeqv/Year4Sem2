# Boost converter CCM capacitor charge-balance equation

## Caption for Word image document
Boost converter CCM charge-balance question: during the switch-on interval the output capacitor alone supplies the load, so iC = −Io; during the switch-off interval the diode conducts and iC = IL − Io. Charge balance gives −δIo + (1−δ)(IL − Io) = 0; correct option A.

## Where this belongs / folder path
`ta questions/Boost convertes/boost-ccm-capacitor-charge-balance-equation.md`

## Question title / short name
Boost CCM capacitor charge-balance equation

## Category
Boost convertes

## Subcategory
Boost converter / CCM charge balance

## Key topic
Using capacitor charge balance over one PWM period to derive the average-current relationship in a boost converter operating in continuous current mode.

## Full visible question text
The circuit diagram below shows a Boost converter.

The voltage and currents in the circuit can be separated into an average quantity and a ripple quantity such that `x(t) = Xbar + Δx(t)`, where `x(t)` is the signal, `Xbar` is the average and `Δx(t)` is the ripple function.

If the circuit is operated in continuous current mode with a duty ratio δ, the charge balance equation for C is given by:

Options shown:
- A: `−δ Io + (1−δ)(IL − Io) = 0`
- B: `−δ Io + (1−δ)IL = 0`
- C: `−δ(IL − Io) + (1−δ)(IL − Io) = 0`
- D: `δ Io + (1−δ)(IL − Io) = 0`

## Given values
- Converter: Boost converter
- Operating mode: CCM
- Duty ratio: `δ`
- Average inductor current: `IL`
- Average output current: `Io`
- Output capacitor: `C`

## What the question is asking for
The correct capacitor charge-balance equation for a boost converter in CCM.

## Correct answer
`A. −δ Io + (1−δ)(IL − Io) = 0`

## Method summary
During Mode 1, the switch is on and the diode is off. The inductor is charged from the input and the capacitor supplies the load, so:

`iC = −Io`

This lasts for duty fraction `δ`.

During Mode 2, the switch is off and the diode is on. The inductor current flows through the diode to the output. Part of this current supplies the load and the remainder charges the capacitor, so:

`iC = IL − Io`

This lasts for duty fraction `1−δ`.

Capacitor charge balance requires the average capacitor current over one switching period to be zero:

`δ(−Io) + (1−δ)(IL − Io) = 0`

Therefore:

`−δ Io + (1−δ)(IL − Io) = 0`

## Formula / equation source
- Formula sheet: capacitor charge balance, `∫ iC dt = 0` over one PWM period in steady state.
- Circuit reasoning: boost Mode 1 has diode off, so the capacitor supplies the load: `iC = −Io`.
- Circuit reasoning: boost Mode 2 has diode on, so the capacitor current is the surplus diode/inductor current after supplying the load: `iC = IL − Io`.

## Must-know concept
For boost charge balance, remember the capacitor is isolated from the inductor during switch-on, so it discharges into the load. During switch-off, the inductor feeds the output and can recharge the capacitor.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded circuit/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic within the archive.

- Manifest check: no existing archived boost converter CCM capacitor charge-balance equation question found.
- Duplicate-logic check: no archived question currently asks for the boost capacitor charge-balance equation using the same Mode 1/Mode 2 capacitor-current reasoning.
- Repository search: no exact repository match found for boost converter charge balance, `−δIo + (1−δ)(IL−Io) = 0`, or the multiple-choice wording.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice question rather than a numerical calculation.
