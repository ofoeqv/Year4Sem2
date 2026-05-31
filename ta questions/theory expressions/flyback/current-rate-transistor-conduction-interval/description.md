# Flyback converter current rate during transistor conduction interval

## Caption for Word image document
Flyback converter theory-expression question: during the transistor conduction interval, the primary winding L1 is connected across the input supply Vdc, so the switch/primary current rises with rate diS/dt = Vdc/L1; correct option A.

## Where this belongs / folder path
`ta questions/theory expressions/flyback/current-rate-transistor-conduction-interval/description.md`

## Question title / short name
Flyback transistor-conduction current rate

## Category
Theory expressions

## Subcategory
Flyback converter / transistor conduction interval

## Key topic
Identifying the rate of change of primary switch current during the flyback transistor on-time.

## Full visible question text
Consider the Flyback converter circuit shown below.

Which one of the following expressions describes the rate of change of current `iS` with respect to time during the transistor conduction interval:

Options shown:
- A: `diS/dt = Vdc/L1`
- B: `diS/dt = Vo/L2`
- C: `diS/dt = 0`
- D: `diS/dt = (Vdc − Vo)/L1`

## Given values
- Converter: Flyback converter
- Interval: transistor conduction interval
- Primary inductance: `L1`
- Secondary inductance: `L2`
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Current of interest: primary/switch current `iS`

## What the question is asking for
The symbolic expression for the rate of change of primary switch current during transistor conduction.

## Correct answer
`A. diS/dt = Vdc/L1`

## Method summary
During the transistor conduction interval, the switch is on. The primary winding/magnetising inductance `L1` is connected directly across the input supply:

`vL1 = Vdc`

Using the inductor equation:

`vL = L di/dt`

For the primary current:

`Vdc = L1 diS/dt`

Therefore:

`diS/dt = Vdc/L1`

During this interval the secondary diode is reverse-biased, so the output side is not controlling the primary current slope.

## Formula / equation source
- Formula sheet: inductor equation, `vL = L di/dt`.
- Circuit reasoning: flyback transistor-on interval applies `Vdc` across primary inductance `L1`.
- Circuit reasoning: the secondary diode is off during transistor conduction.

## Must-know concept
In a flyback converter, the transistor-on interval stores energy in the magnetising inductance. The primary current ramp is set by `Vdc` and `L1`, not by the output voltage.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded multiple-choice screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived question.

## Duplicate-check result
Status: new theory-expression question.

- Repository search found no exact existing archive entry for flyback current rate during the transistor conduction interval.
- Similar existing entry: flyback current rate during the diode conduction interval. That entry asks for `diS/dt = 0` when the transistor is off; this question asks for the transistor-on interval, where `diS/dt = Vdc/L1`.
- Decision: archived as distinct because the conduction interval and correct expression are different.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
