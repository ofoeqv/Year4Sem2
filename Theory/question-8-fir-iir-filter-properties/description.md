# Question 8 - FIR and IIR Filter Properties

## Category
Theory

## Topic
FIR and IIR filters

## Question
Which of the following statements, concerning finite impulse response (FIR) and infinite impulse response (IIR) filters, are true?

## Options
A. FIR filters are always stable

B. Stability can be difficult to judge for IIR filters because quantisation error can cause instability

C. FIR filters need to be lower order for a given filter specification

D. FIR filters can be designed with a perfectly linear phase response

## Correct Answer
A, B and D

## Explanation
A is true. FIR filters have finite impulse responses. If the coefficients are finite, the impulse response is absolutely summable, so the filter is stable.

B is true. IIR filters use feedback, so stability depends on pole locations. Quantisation of coefficients can move poles and may make an IIR filter unstable.

C is false. FIR filters usually need a higher order than IIR filters for the same type of filter specification.

D is true. FIR filters can be designed with exactly linear phase when the impulse response coefficients have the required symmetry.

## Must-know concept
FIR: finite impulse response, no feedback, stable, can have exact linear phase.

IIR: recursive filter with feedback, often lower order, but stability depends on pole positions.

## Duplicate check
Searched the repository for:

- Question 8 FIR IIR filters are true FIR filters always stable quantisation error linear phase
- FIR filters are always stable Stability difficult IIR filters quantisation error can cause instability FIR lower order perfectly linear phase
- Existing path: Theory/question-8-fir-iir-filter-properties/description.md

No duplicate was found before archiving.

## Source
Original uploaded image filename: image.png

## Date archived
2026-06-08
