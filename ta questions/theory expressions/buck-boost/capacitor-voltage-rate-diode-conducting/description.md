# Buck-boost converter capacitor voltage rate when diode conducts

## Caption for Word image document
Buck-boost converter theory-expression question: when the diode conducts, the inductor supplies the output node and the capacitor current is the difference between inductor current and load current, so dvC/dt = (iL − Io)/C; correct option B.

## Where this belongs / folder path
`ta questions/theory expressions/buck-boost/capacitor-voltage-rate-diode-conducting/description.md`

## Question title / short name
Buck-boost capacitor voltage slope during diode conduction

## Category
Theory expressions

## Subcategory
Buck-boost converter / capacitor voltage rate / diode conduction interval

## Key topic
Identifying the capacitor voltage rate of change in an inverting buck-boost converter when the diode is conducting.

## Full visible question text
The circuit diagram below shows a Buck-Boost converter.

Which expression below describes the rate of change of capacitor voltage with respect to time when the diode is conducting?

Options shown:
- A: `dvC/dt = Io/C`
- B: `dvC/dt = (iL − Io)/C`
- C: `dvC/dt = iL/C`
- D: `dvC/dt = (Io − iL)/C`

## Given values
- Converter: Buck-Boost converter
- Diode state: conducting
- Inductor current: `iL`
- Load current: `Io`
- Capacitor: `C`

## What the question is asking for
The symbolic expression for `dvC/dt` during the diode conduction interval.

## Correct answer
`B. dvC/dt = (iL − Io)/C`

## Method summary
Use the capacitor equation:

`iC = C dvC/dt`

During diode conduction, the inductor is delivering current to the output side. The load takes current `Io`. The remaining current goes into the capacitor using the sign convention shown in the diagram:

`iC = iL − Io`

Therefore:

`dvC/dt = (iL − Io)/C`

## Formula / equation source
- Formula sheet: `iC = C dvC/dt`.
- Circuit reasoning: during the buck-boost diode conduction interval, inductor current is transferred to the output side and splits between the capacitor and the load.

## Must-know concept
When the diode conducts in a buck-boost converter, the inductor is feeding the output. If `iL > Io`, the capacitor charges; if `iL < Io`, the capacitor discharges.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a new distinct diode-conduction capacitor-voltage-rate question.

- Similar existing entry: `ta questions/theory expressions/buck-boost/capacitor-voltage-rate-switch-conducting/description.md` asks for the capacitor voltage rate when the switch conducts, with answer `dvC/dt = Io/C`.
- This question asks for the diode conduction interval, where inductor current contributes to the output-side current balance, so the answer is different: `(iL − Io)/C`.
- Repository search found no exact existing archive entry for buck-boost capacitor voltage rate during diode conduction.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question. The sign follows the current and capacitor-voltage reference directions shown in the diagram.
