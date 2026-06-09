# Question 5 - Aliasing with Sampling Period T = 0.1 s

## Category
Theory

## Topic
Sampling theorem and aliasing

## Question
Tick any of the following signals that will suffer from aliasing when sampled at a rate T = 0.1 seconds per sample.

## Options
A. cos(20πt)

B. sin(100t)

C. cos(20t)

D. sin(5πt)

## Correct Answer
A and B

## Explanation
The sampling period is:

\[
T = 0.1 \text{ s}
\]

So the sampling frequency is:

\[
f_s = \frac{1}{T} = \frac{1}{0.1} = 10 \text{ Hz}
\]

The Nyquist frequency is:

\[
f_N = \frac{f_s}{2} = 5 \text{ Hz}
\]

Any signal frequency above 5 Hz will alias.

Option A:

\[
\cos(20\pi t)
\]

Here \(\omega = 20\pi\), so:

\[
f = \frac{\omega}{2\pi} = \frac{20\pi}{2\pi} = 10\text{ Hz}
\]

10 Hz is above 5 Hz, so it aliases.

Option B:

\[
\sin(100t)
\]

Here \(\omega = 100\), so:

\[
f = \frac{100}{2\pi} \approx 15.9\text{ Hz}
\]

15.9 Hz is above 5 Hz, so it aliases.

Option C:

\[
\cos(20t)
\]

Here \(\omega = 20\), so:

\[
f = \frac{20}{2\pi} \approx 3.18\text{ Hz}
\]

3.18 Hz is below 5 Hz, so it does not alias.

Option D:

\[
\sin(5\pi t)
\]

Here \(\omega = 5\pi\), so:

\[
f = \frac{5\pi}{2\pi} = 2.5\text{ Hz}
\]

2.5 Hz is below 5 Hz, so it does not alias.

## Must-know concept
First find the sampling frequency from the sampling period:

\[
f_s = \frac{1}{T}
\]

Then compare signal frequencies to the Nyquist frequency:

\[
f_N = \frac{f_s}{2}
\]

If \(f > f_N\), the signal aliases.

## Duplicate check
Searched the repository for:

- Question 5 signals suffer aliasing sampled rate T 0.1 seconds per sample cos 20 pi t sin 100 t cos 20 t sin 5 pi t
- aliasing sampled at rate T=0.1 seconds per sample cos(20 pi t) sin(100 t)
- Existing path: Theory/question-5-aliasing-sampling-period-0-1s/description.md

No duplicate was found before archiving.

## Source
Original uploaded image filename: image.png

## Date archived
2026-06-09
