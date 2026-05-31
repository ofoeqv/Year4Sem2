# Buck converter inductor current rate when neither switch nor diode conducts

## Caption for Word image document
Buck converter theory-expression question: when neither the switch nor the diode is conducting, the converter is in DCM Mode 3, the inductor current is already zero, and so diL/dt = 0; correct option D.

## Where this belongs / folder path
`ta questions/theory expressions/buck/inductor-current-rate-neither-switch-nor-diode-conducting/description.md`

## Question title / short name
Buck inductor current slope when neither switch nor diode conducts

## Category
Theory expressions

## Subcategory
Buck converter / DCM no-conduction interval

## Key topic
Identifying the inductor current rate of change during the buck converter discontinuous-current Mode 3 interval.

## Full visible question text
The circuit diagram below shows a Buck converter.

Which expression below describes the rate of change of inductor current when neither the switch or the diode is conducting?

Options shown:
- A: `diL/dt = (Vdc − Vo)/L`
- B: `diL/dt = −Vo/L`
- C: `diL/dt = Vdc/L`
- D: `diL/dt = 0`

## Given values
- Converter: Buck converter
- Switch state: not conducting
- Diode state: not conducting
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Inductor: `L`

## What the question is asking for
The symbolic expression for `diL/dt` when both the switch and diode are off.

## Correct answer
`D. diL/dt = 0`

## Method summary
In a buck converter, the normal CCM intervals are:

- Mode 1: switch on, diode off, `vL = Vdc − Vo`, so `diL/dt = (Vdc − Vo)/L`.
- Mode 2: switch off, diode on, `vL = −Vo`, so `diL/dt = −Vo/L`.

If neither the switch nor the diode is conducting, the converter is in DCM Mode 3. The inductor current has already fallen to zero. Since an ideal diode would conduct if the inductor tried to drive current negative, the inductor current remains clamped at zero:

`iL = 0`

Therefore:

`diL/dt = 0`

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: when both switch and diode are off in DCM Mode 3, the inductor current is zero and cannot continue decreasing through the diode path.

## Must-know concept
In DCM Mode 3, the inductor is empty. No switch path and no diode path means the inductor current stays at zero, so the slope is zero.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a new distinct theory-expression question.

- Manifest check: existing buck DCM graph entry asks for diode conduction time, not the inductor current slope in Mode 3.
- Repository search: no exact repository match found for buck converter inductor current rate when neither switch nor diode conducts, `diL/dt = 0`, or the no-conduction DCM interval wording.
- Duplicate-logic check: not a duplicate of buck ON/OFF slope questions because this specifically asks for the DCM no-conduction interval.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
