# Buck converter average switch current expression

## Caption for Word image document
Buck converter theory-expression question: in CCM the switch conducts only during the duty interval δ, and the average inductor current is equal to the output current Io, so the average switch current is Is = Ioδ; correct option B.

## Where this belongs / folder path
`ta questions/theory expressions/buck/average-switch-current-ccm-duty-output-current/description.md`

## Question title / short name
Buck average switch current in CCM

## Category
Theory expressions

## Subcategory
Buck converter / average switch current

## Key topic
Finding the average switch current in a buck converter operating in continuous conduction mode.

## Full visible question text
Question 10.

Assuming a Buck converter is operating in continuous conduction mode with a duty ratio `δ` and an output current `Io`, which of the following expressions correctly describes the average switch current?

Options shown:
- A: `Isbar = Io(1−δ)`
- B: `Isbar = Ioδ`
- C: `Isbar = Io/δ`
- D: `Isbar = Io/(1−δ)`

## Given values
- Converter: Buck converter
- Operating mode: CCM
- Duty ratio: `δ`
- Output current: `Io`
- Requested quantity: average switch current `Isbar`

## What the question is asking for
The correct symbolic expression for the average switch current in a buck converter operating in CCM.

## Correct answer
`B. Isbar = Ioδ`

## Method summary
In a buck converter operating in CCM, the average inductor current is equal to the output current:

`ILbar = Io`

The switch only carries the inductor current during the switch-on interval. The switch is on for duty fraction `δ` of each switching period, and off for `1−δ`.

Therefore, averaged over the full PWM period:

`Isbar = δ ILbar`

Since `ILbar = Io`:

`Isbar = δIo`

## Formula / equation source
- Circuit reasoning: in a buck converter, the switch current equals the inductor current during the on-time and is zero during the off-time.
- Circuit reasoning: in CCM steady state, the average inductor current equals the average output/load current.
- Derived equation: `Isbar = δIo`.

## Must-know concept
The switch does not conduct for the whole period. It carries the load/inductor current only during the duty fraction `δ`, so the average switch current is the output current multiplied by duty ratio.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded multiple-choice screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived question.

## Duplicate-check result
Status: new theory-expression question.

- Repository search found no exact existing archive entry for buck converter average switch current.
- Similar buck theory/balance entries exist, but they ask for charge balance, volt-second balance, boundary conduction, or graph expressions. This one asks specifically for average switch current, so it is a distinct theory-expression category.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
