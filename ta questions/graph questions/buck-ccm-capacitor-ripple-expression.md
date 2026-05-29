# Buck converter CCM capacitor value from ripple waveform

## Caption for Word image document
Graph-based buck converter CCM capacitor-sizing question: the shaded triangular capacitor-current area between inductor current and output current gives the output voltage ripple, so the acceptable filter capacitor condition is C > Tpwm ΔIL / (8 vr(specified)); correct option A.

## Where this belongs / folder path
`ta questions/graph questions/buck-ccm-capacitor-ripple-expression.md`

## Question title / short name
Buck CCM capacitor ripple expression from waveform

## Category
Graph questions

## Subcategory
Buck converter / CCM capacitor ripple expression

## Key topic
Deriving the output capacitor sizing condition from the inductor current ripple waveform and output voltage ripple limit.

## Full visible question text
The waveform below shows waveforms for inductor current IL, output current Io, the output voltage Vo of a Buck converter operating in CCM. The inductor current has a peak-to-peak ripple current of ΔIL and the output voltage has a peak-to-peak ripple of ΔV.

Which one of the following expressions correctly defines an acceptable filter capacitor value to ensure the output voltage ripple does not exceed the specified ripple vr(specified)?

Options shown:
- A: `C > Tpwm ΔIL / (8 vr(specified))`
- B: `C < Tpwm ΔIL / (4 vr(specified))`
- C: `C > Tpwm ΔIL / (4 vr(specified))`
- D: `C < Tpwm ΔIL / (8 vr(specified))`

## Given values
- Converter: Buck converter
- Operating mode: CCM
- Inductor ripple: `ΔIL`
- PWM period: `Tpwm`
- Specified output voltage ripple: `vr(specified)`
- Output capacitor: `C`

## What the question is asking for
The correct inequality for the required output filter capacitor value.

## Correct answer
`A. C > Tpwm ΔIL / (8 vr(specified))`

## Method summary
The capacitor current is the difference between the triangular inductor current and the approximately constant output current. The capacitor charges and discharges over triangular areas. The charge associated with one voltage-ripple excursion gives:

`ΔQ = Tpwm ΔIL / 8`

Using the capacitor relation:

`ΔV = ΔQ / C`

To keep the output voltage ripple below the specified value:

`vr(specified) > Tpwm ΔIL / (8C)`

Rearranging:

`C > Tpwm ΔIL / (8 vr(specified))`

## Formula / equation source
- Formula sheet: `iC = C dvC/dt`, equivalent to `ΔQ = C ΔV`.
- Circuit reasoning: in a buck converter, `iC = iL − Io`, so the capacitor current is the ripple component of inductor current.
- Waveform reasoning: triangular charge area gives the factor of `1/8`.

## Must-know concept
For a buck converter in CCM, capacitor voltage ripple comes from the area under the capacitor-current ripple waveform. The `8` comes from the triangular geometry of the charge/discharge areas.

## Date archived
2026-05-29

## Original image filename
`image.png` from user-uploaded graph/options screenshots.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic within the archive.

- Manifest check: no existing archived graph question for buck CCM capacitor ripple expression.
- Duplicate-logic check: no archived question currently asks for the capacitor-sizing inequality from a buck converter ripple waveform.
- Repository search: no exact repository match found for buck capacitor ripple expression, `Tpwm ΔIL / (8 vr(specified))`, or the graph-based multiple-choice wording.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice graph question rather than a numerical calculation.
