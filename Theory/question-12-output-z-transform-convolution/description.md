# Question 12 - Output Z-transform from Impulse Response and Input

## Category
Theory

## Topic
Z-transform, system function, and LTI output

## Question
Tick the output Z-transform that matches the impulse response:

h[n] = [1 2 3]

when it is fed the input:

x[n] = [4 5 6]

## Options
A. Y(z) = (1 + 2z^-1 + 3z^-2)(4 + 5z^-1 + 6z^-2)

B. Y(z) = (1 + 2z + 3z^2)(4 + 5z + 6z^2)

C. Y(z) = (3 + 2z^-1 + z^-2)(6 + 5z^-1 + 4z^-2)

D. Y(z) = (1 + 2z^-1 + 3z^-2) + (4 + 5z^-1 + 6z^-2)

## Correct Answer
A. Y(z) = (1 + 2z^-1 + 3z^-2)(4 + 5z^-1 + 6z^-2)

## Explanation
For an LTI digital system:

\[
Y(z) = H(z)X(z)
\]

The impulse response:

\[
h[n] = [1, 2, 3]
\]

has Z-transform:

\[
H(z) = 1 + 2z^{-1} + 3z^{-2}
\]

The input:

\[
x[n] = [4, 5, 6]
\]

has Z-transform:

\[
X(z) = 4 + 5z^{-1} + 6z^{-2}
\]

Therefore:

\[
Y(z) = (1 + 2z^{-1} + 3z^{-2})(4 + 5z^{-1} + 6z^{-2})
\]

This matches option A.

## Must-know concept
For an LTI system, convolution in time becomes multiplication in the Z-domain:

\[
y[n] = x[n] * h[n] \quad \Longleftrightarrow \quad Y(z) = X(z)H(z)
\]

## Duplicate check
Searched the repository for:

- Question 12 z-transform impulse response h n 1 2 3 input x n 4 5 6 output z-transform
- Y z 1 2 z inverse 1 3 z inverse 2 4 5 z inverse 1 6 z inverse 2
- Existing path: Theory/question-12-output-z-transform-convolution/description.md

No exact duplicate was found before archiving. Other Question 12 entries exist, but they are on different DSP theory topics, so this was archived separately.

## Source
Original uploaded image filename: image.png

## Date archived
2026-06-08
