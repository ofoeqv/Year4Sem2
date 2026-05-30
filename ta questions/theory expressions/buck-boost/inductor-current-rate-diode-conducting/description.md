# Buck-boost converter inductor current rate when diode is conducting

## Caption for Word image document
Buck-boost converter theory-expression question: when the diode conducts, the inductor discharges into the output and its voltage is Vo using the diagram polarity, so diL/dt = Vo/L; correct option B.

## Where this belongs / folder path
`ta questions/theory expressions/buck-boost/inductor-current-rate-diode-conducting/description.md`

## Question title / short name
Buck-boost inductor current slope during diode conduction

## Category
Theory expressions

## Subcategory
Buck-boost converter / diode conduction interval

## Key topic
Identifying the inductor current rate of change when the diode conducts in an inverting buck-boost converter.

## Full visible question text
The circuit diagram below shows a Buck-Boost converter.

Which expression below describes the rate of change of inductor current with respect to time when the diode is conducting?

Options shown:
- A: `diL/dt = (Vdc − Vo)/L`
- B: `diL/dt = Vo/L`
- C: `diL/dt = Vdc/L`
- D: `diL/dt = (Vo − Vdc)/L`

## Given values
- Converter: Buck-Boost converter
- Diode state: conducting
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Inductor: `L`

## What the question is asking for
The symbolic expression for `diL/dt` during the diode conduction interval.

## Correct answer
`B. diL/dt = Vo/L`

## Method summary
When the switch is off and the diode conducts, the inductor releases its stored energy to the output. Using the voltage and current reference directions shown in the question, the inductor voltage during this interval is:

`vL = Vo`

Using the inductor relation:

`vL = L diL/dt`

Therefore:

`diL/dt = Vo/L`

For the usual inverting buck-boost sign convention, `Vo` is negative, so this expression represents a negative current slope even though it is written as `Vo/L`.

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: during diode conduction, the inductor is connected to the output and discharges its energy to the load/capacitor.

## Must-know concept
In a buck-boost converter, the sign of `Vo` matters. Written with signed output voltage, the diode-conduction slope is `Vo/L`; since the output is negative for the inverting buck-boost, the inductor current is falling.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new theory-expression question. Repository search found no exact existing archive entry for buck-boost inductor current slope during diode conduction.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question. The answer depends on the signed-voltage convention used by the diagram.
