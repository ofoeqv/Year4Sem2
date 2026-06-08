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
**C. The maximum input signal frequency**

## Explanation
In the course sampling-theorem wording, the input signal is bandlimited with highest nonzero angular frequency \(\omega_N\). This \(\omega_N\) is called the **Nyquist frequency**.

The sampling frequency must satisfy:

\[
\omega_s \geq 2\omega_N
\]

The value \(2\omega_N\) is the **Nyquist rate**, not the Nyquist frequency.

## Important note
Some texts also use “Nyquist frequency” to mean half the sampling frequency, \(f_s/2\). However, for this question and the course wording, the intended answer is **C**, because the Nyquist frequency is the maximum input signal frequency that must be sampled at least twice as fast.

## Why the other options are wrong
A. Half the sampling frequency is a common alternative convention, but not the definition used by the course wording here.

B. Double the maximum input signal frequency is the **Nyquist rate**.

D. The rate at which samples are read into the system is the **sampling frequency**.

## Must-know concept
Nyquist frequency: highest input frequency component, \(f_N\).  
Nyquist rate: minimum sampling frequency, \(2f_N\).  
Sampling condition: \(f_s \geq 2f_N\).

## Duplicate check
Searched the repository for:

- `Nyquist frequency half sampling frequency maximum input signal frequency Nyquist rate`
- `Question 11 Nyquist frequency digital systems`
- `double the maximum input signal frequency rate at which samples are read into the system`
- Existing path: `Theory/question-11-nyquist-frequency-definition/description.md`

No duplicate was found before archiving.

## Source
Original uploaded image filename: `image.png`

## Date archived
2026-06-08
