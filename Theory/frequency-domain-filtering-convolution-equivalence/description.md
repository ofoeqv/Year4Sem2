# Frequency-Domain Filtering and Convolution Equivalence

## Category
Theory

## Topic
LTI systems, convolution, and frequency-domain filtering

## Question
Digital filters can be implemented by convolution of a sequence with a system impulse response, or by a process in the frequency domain. Which of the following correctly describes that process?

## Options
A. Fourier transform the sequence, multiply by the system transfer function, then inverse Fourier transform

B. Multiply the sequence by the system transfer function then inverse Fourier transform

C. Convolve the sequence with the system transfer function then take the Fourier transform

D. Multiply the system transfer function by the system impulse response

## Correct Answer
A. Fourier transform the sequence, multiply by the system transfer function, then inverse Fourier transform

## Explanation
For an LTI digital system, filtering in the time domain is convolution:

\[
y[n] = x[n] * h[n]
\]

In the frequency domain, convolution becomes multiplication:

\[
Y(e^{j\Omega}) = X(e^{j\Omega})H(e^{j\Omega})
\]

So the process is:

1. Take the Fourier transform of the input sequence to get \(X(e^{j\Omega})\)
2. Multiply by the system transfer function/frequency response \(H(e^{j\Omega})\)
3. Take the inverse Fourier transform to get \(y[n]\)

## Why the other options are wrong
B. You cannot directly multiply a time-domain sequence by a frequency-domain transfer function.

C. The system transfer function is a frequency-domain object, so it is not convolved with the time-domain sequence.

D. Multiplying the transfer function by the impulse response mixes frequency-domain and time-domain descriptions incorrectly.

## Must-know concept
Time-domain convolution is equivalent to frequency-domain multiplication.

\[
x[n] * h[n] \quad \Longleftrightarrow \quad X(e^{j\Omega})H(e^{j\Omega})
\]

## Duplicate check
Searched the repository for:

- Digital filters implemented by convolution sequence system impulse response frequency domain Fourier transform multiply system transfer function inverse Fourier transform
- Fourier transform the sequence multiply by the system transfer function then inverse Fourier transform
- Existing path: Theory/frequency-domain-filtering-convolution-equivalence/description.md

No duplicate was found before archiving.

## Source
Question provided as text in chat.

## Date archived
2026-06-09
