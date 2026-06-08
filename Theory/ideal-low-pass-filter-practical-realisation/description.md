# Ideal Low-Pass Filter Practical Realisation

## Category
Theory

## Topic
Ideal filters, causality, and realizability

## Question
Why can't the ideal low pass filter be realised in practice?

## Options
A. Its impulse response is non-causal and of infinite length

B. It results in aliasing

C. It requires a high sample frequency

D. It is unstable

## Correct Answer
**A. Its impulse response is non-causal and of infinite length**

## Explanation
An ideal low-pass filter has a perfect brick-wall frequency response. The inverse Fourier transform of that brick-wall response gives a sinc-type impulse response that extends infinitely in both time directions.

That means the impulse response is:

- **infinite length**, so it would require infinitely many samples/coefficient values to implement exactly;
- **non-causal**, because part of the impulse response exists for negative time/index values, meaning the filter would need future input samples.

Therefore, an ideal low-pass filter cannot be realised exactly in practice. Real filters approximate it using FIR or IIR designs.

## Why the other options are wrong
B. Aliasing is caused by insufficient sampling or overlapping spectral replicas, not by the ideal low-pass filter itself.

C. A high sampling frequency may help practical signal processing, but it is not the reason an ideal low-pass filter is unrealizable.

D. The ideal low-pass filter is not rejected because it is unstable; the main issue is non-causality and infinite impulse response length.

## Must-know concept
A physically realisable digital filter must be causal and implementable with finite resources. Ideal brick-wall filters fail this because their impulse responses are non-causal and infinitely long.

## Duplicate check
Searched the repository for:

- `ideal low pass filter realised practice impulse response non-causal infinite length aliasing unstable`
- `Why can't the ideal low pass filter be realised in practice`
- `non-causal infinite length ideal lowpass filter FIR IIR DSP theory`
- Existing path: `Theory/ideal-low-pass-filter-practical-realisation/description.md`

No duplicate was found before archiving.

## Source
Original uploaded image filename: `image.png`

## Date archived
2026-06-08
