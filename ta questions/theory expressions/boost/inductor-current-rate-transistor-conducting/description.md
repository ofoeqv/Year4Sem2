# Boost converter inductor current rate when transistor is conducting

## Caption for Word image document
Boost converter theory-expression question: when the transistor conducts, the diode is off and the input supply is applied across the inductor, so diL/dt = Vdc/L; correct option C.

## Where this belongs / folder path
`ta questions/theory expressions/boost/inductor-current-rate-transistor-conducting/description.md`

## Question title / short name
Boost inductor current slope during transistor conduction

## Category
Theory expressions

## Subcategory
Boost converter / inductor current slope

## Key topic
Identifying the inductor current rate of change during the boost converter switch-on interval.

## Full visible question text
The circuit diagram below shows a Boost converter.

Which expression below describes the rate of change of inductor current when the transistor is conducting?

Options shown:
- A: `diL/dt = (Vdc − Vo)/L`
- B: `diL/dt = Vo/L`
- C: `diL/dt = Vdc/L`
- D: `diL/dt = 0`

## Given values
- Converter: Boost converter
- Transistor state: conducting / switch on
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Inductor: `L`

## What the question is asking for
The symbolic expression for `diL/dt` when the boost transistor is on.

## Correct answer
`C. diL/dt = Vdc/L`

## Method summary
When the transistor is conducting, the switch node is pulled to the reference rail and the diode is reverse-biased. The inductor is connected directly across the input supply, so:

`vL = Vdc`

Using the inductor equation:

`vL = L diL/dt`

Therefore:

`diL/dt = Vdc/L`

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: boost switch-on mode gives `vL = Vdc`.

## Must-know concept
In boost switch-on mode, the inductor is charging from the input supply. The output is temporarily supplied by the capacitor, so `Vo` does not set the inductor current slope in this interval.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new theory-expression question. Repository search found no exact existing archive entry for boost inductor current slope during transistor conduction.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
