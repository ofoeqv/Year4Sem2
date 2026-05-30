# Buck converter CCM boundary condition from inductor-current waveform

## Caption for Word image document
Graph-based buck converter CCM boundary-condition question: the minimum inductor current is the average/output current minus half the peak-to-peak ripple, so continuous conduction requires Io(min) − ΔIL/2 > 0; correct option A.

## Where this belongs / folder path
`ta questions/graph questions/buck-ccm-boundary-continuous-conduction-condition.md`

## Question title / short name
Buck CCM boundary condition from inductor-current waveform

## Category
Graph questions

## Subcategory
Buck converter / CCM boundary condition

## Key topic
Using the inductor-current waveform to identify the condition for remaining in continuous conduction mode.

## Full visible question text
Question 10. The waveform below shows the inductor current for a Buck converter operating in continuous current mode (CCM) where `ILbar` is the average inductor current which is equal to the output current `Io` and `ΔIL` is the peak-to-peak ripple current.

If `Io(min)` is the minimum load current that the Buck converter is expected to operate with in CCM, which of the inequality below correctly defines the boundary of continuous conduction?

Options shown:
- A: `Io(min) − ΔIL/2 > 0`
- B: `Io(min) − ΔIL/2 < 0`
- C: `−2Io(min) + ΔIL > 0`
- D: `Io(min) − 2ΔIL > 0`

## Given values
- Converter: Buck converter
- Operating mode: CCM
- Average inductor current: `ILbar = Io`
- Peak-to-peak ripple current: `ΔIL`
- Minimum expected load current: `Io(min)`

## What the question is asking for
The correct inequality defining the condition for continuous conduction using the minimum inductor current.

## Correct answer
`A. Io(min) − ΔIL/2 > 0`

## Method summary
The minimum inductor current is the average inductor current minus half the peak-to-peak ripple:

`iL,min = ILbar − ΔIL/2`

For a buck converter in steady state:

`ILbar = Io`

At the minimum load current:

`iL,min = Io(min) − ΔIL/2`

To remain in continuous conduction mode, the inductor current must stay above zero:

`Io(min) − ΔIL/2 > 0`

## Formula / equation source
- Waveform reasoning: the minimum of a triangular ripple waveform is the average value minus half the peak-to-peak ripple.
- Circuit reasoning: for a buck converter in steady state, average inductor current equals output current.
- CCM condition: inductor current must not reach zero.

## Must-know concept
CCM means the inductor current never falls to zero. Boundary conduction occurs when the valley of the inductor-current ripple just touches zero.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded waveform/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new graph question.

- Repository search found no exact existing archive entry for a buck CCM boundary-condition waveform inequality question.
- Similar archive entries exist for buck boundary-conduction numerical calculations, but this one asks for a symbolic waveform inequality, so it is stored under graph questions.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice graph question rather than a numerical calculation.
