# Flyback converter energy transferred per PWM cycle in DCM

## Caption for Word image document
Flyback converter DCM energy-per-cycle question: the load power is Po = Vo²/RL, so the energy transferred per full PWM cycle is W = (Vo²/RL)Tpwm; correct option B.

## Where this belongs / folder path
`ta questions/theory expressions/flyback/energy-transferred-per-pwm-cycle-dcm/description.md`

## Question title / short name
Flyback DCM energy transferred per PWM cycle

## Category
Theory expressions

## Subcategory
Flyback converter / DCM energy per cycle

## Key topic
Identifying the energy transferred per PWM cycle from the output load power and switching period in a flyback converter operating in discontinuous mode.

## Full visible question text
Consider the Flyback converter circuit shown below.

If the circuit is operating in discontinuous mode with a transistor on-time `ton` and PWM period `Tpwm`, which expression below describes the energy transferred per PWM cycle?

Options shown:
- A: `W = (Vdc²/RL)Tpwm`
- B: `W = (Vo²/RL)Tpwm`
- C: `W = (Vo²/RL)ton`
- D: `W = (Vdc/RL)ton`

## Given values
- Converter: Flyback converter
- Operating mode: DCM
- Output voltage: `Vo`
- Load resistance: `RL`
- PWM period: `Tpwm`
- Transistor on-time: `ton`

## What the question is asking for
The symbolic expression for energy transferred per full PWM cycle.

## Correct answer
`B. W = (Vo²/RL)Tpwm`

## Method summary
The average output power delivered to the resistive load is:

`Po = Vo²/RL`

Energy transferred over one full switching period is average power multiplied by the PWM period:

`W = Po Tpwm`

Therefore:

`W = (Vo²/RL)Tpwm`

The transistor on-time `ton` is not used directly in this expression because the question asks for energy per complete PWM cycle, not energy only during the switch-on interval.

## Formula / equation source
- Circuit/power reasoning: resistive-load output power `Po = Vo²/RL`.
- Energy relation: `W = P × t` over one full switching cycle.

## Must-know concept
Energy per switching cycle is average output power multiplied by the switching period. Use `Tpwm`, not `ton`, when the question asks for energy transferred per full PWM cycle.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a new flyback theory-expression question.

- Manifest/repository check: no exact existing archive entry found for flyback converter DCM energy transferred per PWM cycle.
- Similar existing entry: buck-boost converter energy transferred per PWM cycle uses the same output-power times switching-period logic, but this question is a different converter topology: isolated flyback rather than non-isolated buck-boost.
- Decision: archived because flyback energy-per-cycle is a distinct useful revision category under the user’s rules.

## Uncertainty
Option D in the screenshot appears to be `W = (Vdc/RL)ton`; the exact exponent on `Vdc` is visually less important because the correct expression is option B, `W = (Vo²/RL)Tpwm`.
