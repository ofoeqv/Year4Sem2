# Flyback converter current rate during diode conduction interval

## Caption for Word image document
Flyback converter theory-expression question: during the diode conduction interval the transistor is off, so the transistor/primary switch current is zero and its rate of change is diS/dt = 0; correct option C.

## Where this belongs / folder path
`ta questions/theory expressions/flyback/current-rate-diode-conduction-interval/description.md`

## Question title / short name
Flyback current rate during diode conduction interval

## Category
Theory expressions

## Subcategory
Flyback converter / diode conduction interval

## Key topic
Identifying the rate of change of transistor current during the flyback diode conduction interval.

## Full visible question text
Consider the Flyback converter circuit shown below.

Which one of the following expressions describes the rate of change of current with respect to time during the diode conduction interval:

Options shown:
- A: `diS/dt = Vdc/L1`
- B: `diS/dt = Vo/L2`
- C: `diS/dt = 0`
- D: `diS/dt = (Vdc − Vo)/L1`

## Given values
- Converter: Flyback converter
- Interval: diode conduction interval
- Primary inductance: `L1`
- Secondary inductance: `L2`
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Current of interest: switch/primary transistor current `iS`

## What the question is asking for
The symbolic expression for the rate of change of switch/primary transistor current during diode conduction.

## Correct answer
`C. diS/dt = 0`

## Method summary
In a flyback converter, the diode conducts during the switch-off interval. When this happens, the transistor is off and no current flows through the primary switch path:

`iS = 0`

Because the switch current remains zero during this interval:

`diS/dt = 0`

The secondary current changes during diode conduction, but the question is asking about `iS`, the switch/primary current shown in the diagram.

## Formula / equation source
- Circuit reasoning: flyback switch-off interval transfers stored magnetising energy through the secondary diode.
- Circuit reasoning: the transistor is off during diode conduction, so primary switch current is zero.

## Must-know concept
In a flyback converter, primary-side current and secondary-side diode current do not conduct at the same time in ideal operation. When the diode conducts, the transistor current is zero.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new theory-expression question. Repository search found no exact existing archive entry for flyback current rate during diode conduction interval.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question. The interpretation assumes the current symbol in the option is `iS`, the transistor/primary switch current.
