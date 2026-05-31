# Flyback converter diode current rate during diode conduction interval

## Caption for Word image document
Flyback converter theory-expression question: during the diode conduction interval, the secondary winding is clamped by the output voltage and the diode current falls, so diD/dt = −Vo/L2; correct option B.

## Where this belongs / folder path
`ta questions/theory expressions/flyback/diode-current-rate-diode-conduction-interval/description.md`

## Question title / short name
Flyback diode current slope during diode conduction

## Category
Theory expressions

## Subcategory
Flyback converter / diode conduction interval / secondary diode current

## Key topic
Identifying the rate of change of secondary diode current during the flyback converter switch-off energy-transfer interval.

## Full visible question text
Consider the Flyback converter circuit shown below.

Which one of the following expressions describes the rate of change of current `iD` with respect to time during the diode conduction interval:

Options shown:
- A: `diD/dt = Vdc/L1`
- B: `diD/dt = −Vo/L2`
- C: `diD/dt = 0`
- D: `diD/dt = (Vdc − Vo)/L1`

## Given values
- Converter: Flyback converter
- Interval: diode conduction interval
- Primary inductance: `L1`
- Secondary inductance: `L2`
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Current of interest: secondary diode current `iD`

## What the question is asking for
The symbolic expression for the rate of change of diode current during the diode conduction interval.

## Correct answer
`B. diD/dt = −Vo/L2`

## Method summary
During the diode conduction interval, the transistor is off and the stored magnetic energy is transferred through the secondary winding and diode to the output.

The secondary winding is clamped by the output voltage. With the current direction `iD` shown in the question, the diode/secondary current is falling, so the secondary inductor current slope is negative:

`vL2 = −Vo`

Using the inductor relation:

`vL = L di/dt`

therefore:

`diD/dt = −Vo/L2`

## Formula / equation source
- Formula sheet: `vL = L di/dt`.
- Circuit reasoning: during flyback diode conduction, the secondary winding is connected to the output through the diode and the secondary current ramps down as energy is delivered to the load/capacitor.

## Must-know concept
In a flyback converter, diode conduction is the energy-delivery interval. The secondary current starts high and decreases to zero, so the diode current slope must be negative.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a new distinct requested-current question.

- Similar existing entry: `ta questions/theory expressions/flyback/current-rate-diode-conduction-interval/description.md` asks for switch/primary transistor current `iS` during the diode conduction interval, with answer `diS/dt = 0`.
- This question asks for secondary diode current `iD` during the same interval, so the requested current is different and the answer is different.
- Repository search found no exact existing archive entry for flyback diode current rate `diD/dt = −Vo/L2`.
- Decision: archive as a distinct useful revision category.

## Uncertainty
The option is read as `B. diD/dt = −Vo/L2`, which matches the expected falling diode current during the flyback diode conduction interval.
