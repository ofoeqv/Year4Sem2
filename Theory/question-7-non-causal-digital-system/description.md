# Question 7 - Non-causal Digital System

## Category
Theory

## Topic
Causality in digital systems

## Question
A digital system would be considered **non-causal** if it included which of the following operations?

## Options
A. Multiply the input by a constant

B. Square the input sequence (multiply it by itself)

C. Add the current input to the current output

D. Multiply the output by a constant

## Correct Answer
**C. Add the current input to the current output**

## Explanation
A causal digital system can use the present input, past inputs, and past outputs to compute the present output. It must not require future information.

Option C is the only option that suggests using the current output while trying to compute the current output. In implementation terms, this creates an instantaneous/algebraic dependency unless it is rearranged into a valid causal equation.

Strictly speaking, the clearest textbook example of a non-causal system would involve a future sample, such as:

\[
y[n] = x[n+1]
\]

So this question is slightly ambiguous. If forced to choose from the listed options, **C** is the intended answer.

## Why the other options are not non-causal
A. Multiplying the current input by a constant is causal.

B. Squaring the current input is nonlinear, but still causal because it only uses the present input.

D. Multiplying the output by a constant does not by itself imply future dependence.

## Must-know concept
Causal system: output at time \(n\) depends only on present/past inputs and, for recursive systems, past outputs.  
Non-causal system: output at time \(n\) depends on future values such as \(x[n+1]\).

## Duplicate check
Searched the repository for:

- `non-causal digital system included operation multiply input by constant square input sequence add current input current output`
- `Question 7 non-causal digital system operation`
- `causal non-causal current input current output future input DSP theory`
- Existing path: `Theory/question-7-non-causal-digital-system/description.md`

No duplicate was found before archiving. Another Question 7 on DFT exists, but it is a different question/topic, so this was archived separately.

## Source
Original uploaded image filename: `image.png`

## Date archived
2026-06-08
