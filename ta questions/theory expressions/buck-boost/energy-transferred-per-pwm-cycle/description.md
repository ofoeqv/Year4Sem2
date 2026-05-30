# Buck-boost converter energy transferred per PWM cycle

## Caption for Word image document
Buck-boost converter theory-expression question: the load receives energy through the output over each PWM period, so the energy transferred per PWM cycle is W = (Vo²/RL)Tpwm; correct option C.

## Where this belongs / folder path
`ta questions/theory expressions/buck-boost/energy-transferred-per-pwm-cycle/description.md`

## Question title / short name
Buck-boost energy transferred per PWM cycle

## Category
Theory expressions

## Subcategory
Buck-boost converter / energy per cycle

## Key topic
Identifying the energy transferred to the load per PWM cycle from output power and switching period.

## Full visible question text
The circuit diagram below shows a Buck-Boost converter.

If the switch is operated with an on-time `ton`, which expression below describes the energy transferred per PWM cycle?

Options shown:
- A: `W = (Vdc²/L)ton`
- B: `W = (Vo²/RL)Tpwm`
- C: `W = (Vo²/RL)Tpwm`
- D: `W = (Vo²/RL)ton`

## Given values
- Converter: Buck-Boost converter
- Output voltage: `Vo`
- Load resistance: `RL`
- PWM period: `Tpwm`
- Switch on-time: `ton`

## What the question is asking for
The symbolic expression for energy transferred per PWM cycle.

## Correct answer
`C. W = (Vo²/RL)Tpwm`

## Method summary
The average output power delivered to a resistive load is:

`Po = Vo²/RL`

Energy transferred over one switching period is power multiplied by time:

`W = Po Tpwm`

Therefore:

`W = (Vo²/RL)Tpwm`

## Formula / equation source
- Circuit/power reasoning: resistive-load output power `Po = Vo²/RL`.
- Energy relation: `W = P × t`.

## Must-know concept
Energy per switching cycle is average power times switching period. Use `Tpwm`, not just the switch on-time, when the question asks for energy transferred per full PWM cycle.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new theory-expression question. Repository search found no exact existing archive entry for buck-boost energy transferred per PWM cycle.

## Uncertainty
The screenshot appears to show options B and C with the same expression. The selected answer is the expression `W = (Vo²/RL)Tpwm`; if the platform labels one duplicated option differently, use the expression rather than relying only on the letter.
