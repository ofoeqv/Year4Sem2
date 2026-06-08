# Question 13 - Impulse Response and Moving Average

## Category
Theory

## Topic
Impulse response and FIR moving-average systems

## Question
What would be the output of a digital system with the impulse response:

h[n] = [1 1 1 1]/4

Defined for n = 0, 1, 2, 3.

## Options
A. The average of the current and the previous three inputs to the system.

B. The average of the previous four inputs to the system.

C. The average of the previous four outputs from the system.

D. Four times the previous output from the system.

## Correct Answer
A. The average of the current and the previous three inputs to the system.

## Explanation
For an LTI digital system, the output is the convolution of the input with the impulse response:

\[
y[n] = x[n] * h[n]
\]

Since:

\[
h[0] = h[1] = h[2] = h[3] = \frac{1}{4}
\]

then:

\[
y[n] = \frac{1}{4}x[n] + \frac{1}{4}x[n-1] + \frac{1}{4}x[n-2] + \frac{1}{4}x[n-3]
\]

So:

\[
y[n] = \frac{x[n] + x[n-1] + x[n-2] + x[n-3]}{4}
\]

This is the average of the current input and the previous three input samples.

## Must-know concept
An FIR impulse response with equal coefficients acts like a moving-average filter. The coefficient positions tell you which input samples are averaged.

## Duplicate check
Searched the repository for:

- Question 13 impulse response h n 1 1 1 1 over 4 average current previous three inputs
- average current and previous three inputs impulse response moving average FIR h[n]
- Existing path: Theory/question-13-impulse-response-moving-average/description.md

No duplicate was found before archiving.

## Source
Original uploaded image filename: image.png

## Date archived
2026-06-08
