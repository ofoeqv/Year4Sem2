# Question 14 - DFT Linear Convolution Zero Padding

## Category
Theory

## Topic
Discrete Fourier Transform (DFT) and linear convolution

## Question
Two sequences of lengths 5 and 6 are to be **linearly convolved using the DFT**. How many zeros must the length-5 sequence be padded out with?

## Options
A. 5  
B. 6  
C. 4  
D. 11

## Correct Answer
**A. 5**

## Explanation
For linear convolution of two finite-length sequences using the DFT, the DFT length must be at least:

\[
N \geq L + P - 1
\]

Here:

\[
L = 5, \quad P = 6
\]

So:

\[
N \geq 5 + 6 - 1 = 10
\]

The length-5 sequence must therefore be padded to length 10:

\[
10 - 5 = 5
\]

So the length-5 sequence needs **5 zeros**.

## Must-know concept
To use the DFT for **linear** convolution, both sequences must be zero-padded to at least \(L + P - 1\). Otherwise, the DFT gives circular convolution with time-domain wraparound.

## Source
Original uploaded image filename: `image.png`

## Date archived
2026-06-08
