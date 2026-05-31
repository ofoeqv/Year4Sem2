# Buck converter average diode current in CCM

## Caption for Word image document
Buck converter theory-expression question: in CCM, the diode conducts during the switch off-time fraction (1−δ) and carries approximately the output/inductor current, so the average diode current is IDbar = Io(1−δ); correct option A.

## Where this belongs / folder path
`ta questions/theory expressions/buck/average-diode-current-ccm-duty-output-current/description.md`

## Question title / short name
Buck average diode current in CCM

## Category
Theory expressions

## Subcategory
Buck converter / average diode current

## Key topic
Finding the average diode current in a buck converter operating in continuous conduction mode from duty ratio and output current.

## Full visible question text
Question 10.

Assuming a Buck converter is operating in continuous conduction mode with a duty ratio `δ` and an output current `Io`, which of the following expression correctly describes the average diode current?

Options shown:
- A: `IDbar = Io(1−δ)`
- B: `IDbar = Io`
- C: `IDbar = Io/δ`
- D: `IDbar = Io/(1−δ)`

## Given values
- Converter: Buck converter
- Operating mode: CCM
- Duty ratio: `δ`
- Output current: `Io`
- Device of interest: diode `D`

## What the question is asking for
The symbolic expression for the average diode current in a buck converter operating in CCM.

## Correct answer
`A. IDbar = Io(1−δ)`

## Method summary
In a buck converter operating in CCM:

- During switch on-time, the switch conducts and the diode is off.
- During switch off-time, the diode conducts and carries the inductor current.

The off-time fraction is:

`1−δ`

In CCM, the average inductor current is approximately equal to the output current:

`ILbar = Io`

Therefore the average diode current is the current it carries multiplied by the fraction of the PWM period for which it conducts:

`IDbar = Io(1−δ)`

## Formula / equation source
- Circuit reasoning: buck converter diode conducts during the switch off-time interval.
- CCM average-current reasoning: average inductor current equals output current, `ILbar = Io`.

## Must-know concept
In a buck converter, the switch carries the inductor/load current during `δ`, and the diode carries it during `1−δ`. So average switch current is `Ioδ`, while average diode current is `Io(1−δ)`.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a new distinct theory-expression question.

- Similar existing entry: `ta questions/theory expressions/buck/average-switch-current-ccm-duty-output-current/description.md` asks for average switch current, `Isbar = Ioδ`.
- This question asks for average diode current, which occurs during the complementary off-time interval, so the answer is `IDbar = Io(1−δ)`.
- Repository search found no exact existing archive entry for buck converter average diode current in CCM.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
