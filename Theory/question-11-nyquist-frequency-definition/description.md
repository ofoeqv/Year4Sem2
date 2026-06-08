# Question 11 - Nyquist Frequency Definition

## Category
Theory

## Topic
Sampling theorem and Nyquist frequency

## Question
Which is the correct definition of the **Nyquist frequency** in relation to digital systems?

## Options
A. Half the sampling frequency

B. Double the maximum input signal frequency

C. The maximum input signal frequency

D. The rate at which samples are read into the system

## Correct Answer
**A. Half the sampling frequency**

## Explanation
For a digital/sampled system, the **Nyquist frequency** is half the sampling frequency:

\[
f_N = \frac{f_s}{2}
\]

It is the highest frequency that can be represented without aliasing for a sampling rate \(f_s\).

Option B, double the maximum input signal frequency, describes the **Nyquist rate** requirement:

\[
f_s \geq 2f_{max}
\]

Option C is the maximum input signal frequency, which must be less than or equal to the Nyquist frequency for alias-free sampling.

Option D is the sampling frequency itself, \(f_s\), not the Nyquist frequency.

## Important note
Some lecture notes define \(\omega_N\), the highest nonzero input frequency component, as the Nyquist frequency, and call \(2\omega_N\) the Nyquist rate. However, in this quiz wording, **in relation to digital systems**, the intended convention is:

\[
\text{Nyquist frequency} = \frac{f_s}{2}
\]

## Must-know concept
Nyquist frequency: \(f_s/2\).  
Nyquist rate: minimum sampling rate needed to avoid aliasing, \(2f_{max}\).  
Aliasing-free condition: \(f_{max} \leq f_s/2\), equivalently \(f_s \geq 2f_{max}\).

## Duplicate check
Duplicate found at this same path and updated rather than creating a new file:

`Theory/question-11-nyquist-frequency-definition/description.md`

Previous archived answer was corrected from **C** to **A** after the updated screenshot showed option A selected.

## Source
Original uploaded image filename: `image.png`

## Date archived
2026-06-08

## Date corrected
2026-06-08
