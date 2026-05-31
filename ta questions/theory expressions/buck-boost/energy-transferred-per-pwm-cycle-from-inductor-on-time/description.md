# Buck-boost converter energy transferred per PWM cycle from inductor on-time

## Caption for Word image document
Buck-boost converter DCM energy-per-cycle question: during switch on-time the inductor current rises from zero with slope Vdc/L, so the peak current is Ip = Vdc ton/L and the stored/transferred energy is W = 1/2 L Ip² = (Vdc ton)²/(2L); correct option A.

## Where this belongs / folder path
`ta questions/theory expressions/buck-boost/energy-transferred-per-pwm-cycle-from-inductor-on-time/description.md`

## Question title / short name
Buck-boost energy transferred per PWM cycle from inductor on-time

## Category
Theory expressions

## Subcategory
Buck-boost converter / DCM energy per cycle / inductor stored energy

## Key topic
Finding the energy transferred per PWM cycle in a buck-boost converter from the inductor current ramp during switch on-time.

## Full visible question text
The circuit diagram below shows a Buck-Boost converter.

If the switch is operated with an on-time `ton`, which expression below describes the energy transferred per PWM cycle?

Options shown:
- A: `W = (Vdc ton)^2/(2L)`
- B: `W = (Vdc Tpwm)^2/(2L)`
- C: `W = (Vdc(Tpwm − ton))^2/(2L)`
- D: `W = Vdc ton/(2L)`

## Given values
- Converter: Buck-Boost converter
- Switch on-time: `ton`
- Input voltage: `Vdc`
- Inductor: `L`
- PWM period: `Tpwm`

## What the question is asking for
The symbolic expression for the energy transferred per PWM cycle based on the inductor energy built during switch on-time.

## Correct answer
`A. W = (Vdc ton)^2/(2L)`

## Method summary
During switch on-time in a buck-boost converter, the inductor is connected across the input supply:

`vL = Vdc`

Using the inductor relation:

`vL = L diL/dt`

so:

`diL/dt = Vdc/L`

In DCM, the inductor current starts at zero and rises during `ton`, so the peak current is:

`Ip = (Vdc/L) ton`

The energy stored in the inductor at the end of the on-time is:

`W = 1/2 L Ip^2`

Substitute `Ip`:

`W = 1/2 L (Vdc ton/L)^2`

Therefore:

`W = (Vdc ton)^2/(2L)`

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: buck-boost switch-on interval applies `Vdc` across the inductor.
- Derived energy relation: `W = 1/2 L I^2` for energy stored in an inductor.

## Must-know concept
In DCM, the inductor starts empty each cycle. The energy transferred per cycle is the energy stored in the inductor during switch on-time, so it depends on `ton`, not `Tpwm − ton`.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a distinct buck-boost energy question.

- Similar existing entry: `ta questions/theory expressions/buck-boost/energy-transferred-per-pwm-cycle/description.md` uses output-load power, `W = (Vo²/RL)Tpwm`.
- This question uses the inductor ramp from switch on-time and the stored-energy equation, `W = 1/2 L I²`, giving `W = (Vdc ton)^2/(2L)`.
- Same converter family and broad energy theme, but different equation/toolset and different solution method, so it is not duplicate logic.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
