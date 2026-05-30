# Feedback controller output voltage from divider feedback gain

## Caption for Word image document
Feedback-style power-supply controller question: for a large forward DC gain, the feedback signal is approximately equal to the reference signal. With H(0) = R2/(R1 + R2), R1 = 5 kΩ, R2 = 5 kΩ, and reference r = 2.5 V, the output voltage is y = 5.00 V.

## Where this belongs / folder path
`ta questions/feedback style/feedback-controller-output-voltage-divider-r1-5k-r2-5k-r-2p5v/description.md`

## Question title / short name
Feedback controller output voltage from potential-divider feedback

## Category
Feedback style

## Subcategory
Negative feedback / DC closed-loop output voltage

## Key topic
Using large-loop-gain negative feedback and a potential-divider feedback gain to find the regulated power-supply output voltage.

## Full visible question text
The block diagram below shows a simplified representation of a power supply feedback controller. The power supply reference signal is `r`, the power supply output is `y`, `G(s)` is the forward gain and `H(s)` is the feedback gain.

For DC conditions the forward gain is very large `G(s=0) >> 1` and the feedback gain is obtained using a potential divider constructed using two resistors `R1` and `R2` and has a transfer function given by `H(s) = R2/(R1 + R2)`. If the reference signal `r = 2.5 V` and the resistor value are `R1 = 5 kΩ` and `R2 = 5 kΩ`, what is the power supply output voltage?

Please specify your answer in units of V to 2 decimal places.

## Given values
- Reference signal: `r = 2.5 V`
- Forward DC gain: `G(0) >> 1`
- Feedback gain: `H(0) = R2/(R1 + R2)`
- `R1 = 5 kΩ`
- `R2 = 5 kΩ`

## What the question is asking for
The regulated power-supply output voltage `y`, in volts.

## Correct answer
`y = 5.00 V`

## Method summary
For negative feedback, the error is:

`e = r − H y`

The output is:

`y = G e = G(r − H y)`

Rearrange:

`y(1 + GH) = Gr`

so the closed-loop gain is:

`y/r = G/(1 + GH)`

For very large DC forward gain, `G(0) >> 1`, this becomes approximately:

`y/r ≈ 1/H`

The feedback divider is:

`H = R2/(R1 + R2) = 5/(5 + 5) = 0.5`

Therefore:

`y = r/H = 2.5/0.5 = 5.00 V`

## Formula / equation source
- Control-system feedback relation: `y/r = G/(1 + GH)` for negative feedback.
- Large-gain approximation: when `G >> 1`, the output adjusts so `Hy ≈ r`.
- Circuit reasoning: potential-divider feedback gain `H = R2/(R1 + R2)`.

## Must-know concept
With high-gain negative feedback, the feedback signal is forced to match the reference. If the divider feeds back half the output, then the output must be twice the reference.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded block-diagram screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, similar feedback concept but not duplicate logic.

- Manifest check: existing feedback-related entries concern closed-loop buck converter circuit questions, including `Vdc` from PWM/C2, voltage across C9, and beta from bias current. This question uses a generic feedback block diagram and asks for output voltage from `H = R2/(R1 + R2)` and large forward gain.
- Duplicate-logic check: not treated as duplicate logic because the requested element and toolset differ from the archived closed-loop buck circuit calculations.
- Repository search: no exact repository match found for generic feedback controller output voltage, `H = R2/(R1 + R2)`, `R1 = 5 kΩ`, `R2 = 5 kΩ`, and `r = 2.5 V`.

## Uncertainty
No visible value uncertainty. The prompt clearly gives `r = 2.5 V`, `R1 = 5 kΩ`, `R2 = 5 kΩ`, and `G(0) >> 1`.
