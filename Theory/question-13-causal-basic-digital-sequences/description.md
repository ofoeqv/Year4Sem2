# Question 13 - Causal Basic Digital Sequences

## Category
Theory

## Topic
Causal sequences in discrete-time systems

## Question
Which of the following basic digital sequences are causal?

## Options
A. u[n](0.2)^(n+3)

B. u[n+2](0.2)^n

C. (0.2)^(n-1)

D. 2^n

## Correct Answer
A. u[n](0.2)^(n+3)

## Explanation
A causal discrete-time sequence is zero for all negative time indices:

\[
x[n] = 0 \quad \text{for } n < 0
\]

Option A contains u[n], so the sequence only starts at n = 0. Therefore it is causal:

\[
u[n](0.2)^{n+3} = 0 \quad \text{for } n < 0
\]

Option B contains u[n+2], which starts at n = -2, so it has nonzero samples before n = 0. Therefore it is not causal.

Options C and D are plain exponential sequences with no unit step limiting them to n >= 0, so they are generally nonzero for negative n. Therefore they are not causal.

## Must-know concept
A causal sequence must be right-sided: it is zero before n = 0. A unit step u[n] makes a sequence causal, but u[n+2] starts early at n = -2, so it is non-causal.

## Duplicate check
Searched the repository for:

- Question 13 basic digital sequences are causal u n 0.2 n plus 3 u n plus 2 exponential
- causal sequence u[n] u[n+2] 0.2 exponentials DSP theory
- Existing path: Theory/question-13-causal-basic-digital-sequences/description.md

No exact duplicate was found before archiving. Other Question 13 entries exist, but they are on different DSP theory topics, so this was archived separately.

## Source
Original uploaded image filename: image.png

## Date archived
2026-06-08
