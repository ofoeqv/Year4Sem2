# Boost converter maximum transistor voltage expression

## Caption for Word image document
Boost converter theory-expression question: when the transistor is off, the diode conducts and clamps the switch node to the output, so the maximum transistor voltage during normal operation is Vo; correct option B.

## Where this belongs / folder path
`ta questions/theory expressions/boost/maximum-transistor-voltage-normal-operation/description.md`

## Question title / short name
Boost maximum transistor voltage

## Category
Theory expressions

## Subcategory
Boost converter / transistor voltage stress

## Key topic
Identifying the maximum switch voltage in a boost converter during normal operation.

## Full visible question text
The circuit diagram below shows a Boost converter.

What is the maximum voltage the transistor will experience during normal operation?

Options shown:
- A: `Vdc`
- B: `Vo`
- C: `Vo − Vdc`
- D: `Vo + Vdc`

## Given values
- Converter: Boost converter
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Device of interest: transistor/switch

## What the question is asking for
The symbolic expression for the maximum transistor voltage during normal boost operation.

## Correct answer
`B. Vo`

## Method summary
In a boost converter, when the transistor is off, the inductor current flows through the diode into the output. The switch node is then clamped approximately to the output voltage. Since the lower terminal of the transistor is at the reference rail, the transistor voltage stress is approximately:

`vS,max = Vo`

## Formula / equation source
- Circuit reasoning: boost switch-off interval clamps the switch node to the output through the diode.
- Device voltage-stress reasoning: the transistor must block the output voltage when off.

## Must-know concept
In a boost converter, the switch voltage stress is set by the output voltage, not just the input voltage.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new theory-expression question. Repository search found no exact existing archive entry for boost maximum transistor voltage.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
