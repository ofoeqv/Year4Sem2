# Flyback converter energy transferred per PWM cycle in DCM

## Caption for Word image document
Flyback converter DCM energy-per-cycle question: during transistor on-time the primary magnetising current rises from zero with slope Vdc/L1, so the peak current is Ip = Vdc ton/L1 and the stored/transferred energy is W = 1/2 L1 Ip² = (Vdc ton)²/(2L1); correct option A.

## Where this belongs / folder path
`ta questions/theory expressions/flyback/energy-transferred-per-pwm-cycle-dcm/description.md`

## Question title / short name
Flyback DCM energy transferred per PWM cycle from primary magnetising energy

## Category
Theory expressions

## Subcategory
Flyback converter / DCM energy per cycle / magnetising inductance stored energy

## Key topic
Finding the energy transferred per PWM cycle in a flyback converter operating in discontinuous mode from the primary magnetising current ramp during transistor on-time.

## Full visible question text
Consider the Flyback converter circuit shown below.

If the circuit is operating in discontinuous mode with a transistor on-time `ton` and PWM period `Tpwm`, which expression below describes the energy transferred per PWM cycle?

Options shown:
- A: `W = (Vdc ton)^2/(2L1)`
- B: `W = (Vdc Tpwm)^2/(2L1)`
- C: `W = Vdc Tpwm/(2L1)`
- D: `W = (Vdc ton)^2/L1`

## Given values
- Converter: Flyback converter
- Operating mode: DCM
- Input voltage: `Vdc`
- Primary/magnetising inductance: `L1`
- Transistor on-time: `ton`
- PWM period: `Tpwm`

## What the question is asking for
The symbolic expression for energy transferred per PWM cycle based on the energy stored in the primary magnetising inductance during transistor on-time.

## Correct answer
`A. W = (Vdc ton)^2/(2L1)`

## Method summary
During transistor on-time, the flyback primary magnetising inductance is connected across the input supply:

`vL1 = Vdc`

Using the inductor equation:

`vL = L di/dt`

so the primary current slope is:

`diS/dt = Vdc/L1`

In DCM, the magnetising current starts from zero each cycle. Therefore, after `ton`, the peak primary current is:

`Ip = (Vdc/L1)ton`

The energy stored in the magnetising inductance at the end of transistor on-time is:

`W = 1/2 L1 Ip^2`

Substitute the peak current:

`W = 1/2 L1 (Vdc ton/L1)^2`

Therefore:

`W = (Vdc ton)^2/(2L1)`

## Formula / equation source
- Formula sheet: `vL = L di/dt`.
- Derived circuit reasoning: flyback transistor-on interval applies `Vdc` across primary magnetising inductance `L1`.
- Derived energy relation: energy stored in an inductor, `W = 1/2 L I^2`.

## Must-know concept
A DCM flyback stores energy in the primary magnetising inductance during transistor on-time, then transfers that stored energy to the secondary during diode conduction. The energy per cycle is set by the peak magnetising current, so it depends on `ton`, `Vdc`, and `L1`.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: corrected and archived as the flyback DCM magnetising-energy question.

- This replaces an earlier description that incorrectly treated the question as an output-load-power-per-period expression.
- Similar existing entry: buck-boost converter inductor-energy per cycle uses the same stored-energy method, but this question is a flyback topology and uses the primary magnetising inductance `L1`.
- Decision: keep this as the flyback-specific DCM energy-per-cycle entry.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question. The answer is based on DCM operation where the primary magnetising current starts from zero each cycle.
