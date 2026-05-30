# Buck-boost converter capacitor voltage rate when switch is conducting

## Caption for Word image document
Buck-boost converter theory-expression question: when the switch is conducting, the diode is off and the output capacitor alone supplies the load, so the capacitor voltage changes at a rate set by the load current; with the voltage polarity used in the options, dvC/dt = Io/C, correct option A.

## Where this belongs / folder path
`ta questions/theory expressions/buck-boost/capacitor-voltage-rate-switch-conducting/description.md`

## Question title / short name
Buck-boost capacitor voltage rate during switch conduction

## Category
Theory expressions

## Subcategory
Buck-boost converter / capacitor voltage slope

## Key topic
Identifying the capacitor voltage rate of change during the switch-on interval of an inverting buck-boost converter.

## Full visible question text
The circuit diagram below shows a Buck-Boost converter.

Which expression below describes the rate of change of capacitor voltage with respect to time when the switch is conducting?

Options shown:
- A: `dvC/dt = Io/C`
- B: `dvC/dt = (iL − Io)/C`
- C: `dvC/dt = iL/C`
- D: `dvC/dt = (Io − iL)/C`

## Given values
- Converter: Buck-Boost converter
- Switch state: conducting / switch on
- Diode state: off
- Output current: `Io`
- Inductor current: `iL`
- Output capacitor: `C`

## What the question is asking for
The symbolic expression for the rate of change of capacitor voltage during the switch-on interval.

## Correct answer
`A. dvC/dt = Io/C`

## Method summary
When the switch is conducting in an inverting buck-boost converter, the diode is reverse-biased. The inductor is being charged from the input supply and is not feeding the output.

Therefore the output capacitor alone supplies the load during this interval.

Using the capacitor relation:

`iC = C dvC/dt`

and the voltage/current polarity convention used by the answer options, the capacitor voltage rate is set only by the load current:

`dvC/dt = Io/C`

The inductor current does not appear in the expression because the diode is off, so the inductor is disconnected from the output during switch conduction.

## Formula / equation source
- Formula sheet: capacitor equation, `iC = C dvC/dt`.
- Circuit reasoning: during buck-boost switch-on mode, the diode is off and the output capacitor supplies the load.

## Must-know concept
During buck-boost switch-on time, the output side is isolated from the inductor. The capacitor is the only element feeding the load, so the capacitor-voltage slope depends on `Io`, not `iL`.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded multiple-choice screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived question.

## Duplicate-check result
Status: new theory-expression question.

- Repository search found no exact existing archive entry for buck-boost capacitor voltage rate during switch conduction.
- Similar entries exist for buck-boost capacitor charge balance and buck-boost inductor current slope during diode conduction, but this question asks for a different element: capacitor voltage slope during switch-on operation.
- Decision: archived under `theory expressions/buck-boost` as a distinct theory-expression category.

## Uncertainty
No numerical uncertainty. Note that the sign depends on the voltage polarity convention. The answer options use the convention for which the intended expression is `dvC/dt = Io/C`.
