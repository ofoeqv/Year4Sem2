# Impulse Response Definition

## Category
Theory

## Topic
Digital systems and impulse response

## Question
Choose the correct definition of the **impulse response** of a digital system.

## Options
A. The output of the system when the input is a unit impulse.

B. The output of the system when the input is an analogue delta function.

C. The convolution of the input and output of the system.

D. The sum of the shifted input to the system.

## Correct Answer
**A. The output of the system when the input is a unit impulse.**

## Explanation
The impulse response of a discrete-time/digital system is the output produced when the input is the unit impulse sequence:

\[
\delta[n]
\]

For an LTI system, the impulse response is usually written as:

\[
h[n]
\]

and it fully characterises the system because any output can be found by convolution:

\[
y[n] = x[n] * h[n]
\]

Option B is wrong because an analogue delta function belongs to continuous-time systems, not digital/discrete-time systems. Option C is wrong because the output is the convolution of the input with the impulse response, not the convolution of the input and output. Option D is not the definition of impulse response.

## Must-know concept
Impulse response = system output when the input is \(\delta[n]\). For an LTI system, knowing \(h[n]\) tells you the full behaviour of the system.

## Duplicate check
Searched the repository for:

- `impulse response digital system unit impulse output system input unit impulse`
- `Choose the correct definition of the impulse response of a digital system`
- Existing path: `Theory/impulse-response-definition/description.md`

No duplicate was found before archiving.

## Source
Original uploaded image filename: `image.png`

## Date archived
2026-06-08
