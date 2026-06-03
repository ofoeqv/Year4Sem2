# Quiz 5 - Photodetectors

Source: Quiz5AnswersWhole.pdf

## Question 1
Consider a p-i-n photodiode with an absorption region of 1.5 x 10^-6 m.

What is the photocurrent produced when a GaAs laser, with a wavelength of 870 nm and an optical power of 0.0006 W, is focused on this photodiode?

The absorption coefficient at this wavelength is 700 cm^-1. Express your answer in A. Assume no reflection at the surface. Round your answer to 2 decimal places.

Answer: 4.03E-5 A **[correct]**

Accepted range: 4.03E-5 ± 10%

Feedback/formulas:

- Fraction of light absorbed = 1 - exp(-alpha W)
- Responsivity R = [1 - exp(-alpha W)] x 0.87 / 1.24
- Current = Responsivity x Power = R x P

## Question 2
An avalanche photodiode is expected to produce a photocurrent of 10.2 nA under unity gain condition.

If the incident optical power is 108 nW and the wavelength is 874 nm, what is the required quantum efficiency? Express your answer in %. Round your answer to 2 decimal places.

Answer: 13.40% **[correct]**

Accepted range: 13.40 ± 5%

Feedback/formula:

R = Iph / P = eta lambda / 1.24

## Question 3
An extremely fast photodiode can be designed to achieve bandwidth of 158 GHz.

Assuming that the bandwidth is limited by carrier transit time, calculate the required depletion region if the electron and hole saturation velocities are 0.85 x 10^5 m s^-1.

Express your answer in micrometres. Round your answer to 2 decimal places.

Answer: 0.22 um **[correct]**

Accepted range: 0.22 ± 10%

Feedback/formula:

Transit-time limited bandwidth: f = 0.4 / tau = 0.4v / W

## Question 4
Consider an In0.53Ga0.47As waveguide photodiode with an RC-limited bandwidth of 62 GHz.

Assuming R = 67 ohm, calculate the capacitance of the photodiode. Express your answer in pF. Round your answer to 3 decimal places.

Answer: 0.038 pF **[correct]**

Accepted range: 0.038 ± 10%

Feedback/formula:

RC-limited bandwidth: f = 1 / (2 pi R C)

## Question 5
A high-speed photodiode has a width of 6.2 um and a length of 84 um.

The RC time constant of this photodiode is 31.83 ps. What is the depletion width for this photodiode if R = 50 ohm and the relative dielectric constant of In0.53Ga0.47As is 13.9?

Express your answer in micrometres. Round your answer to 2 decimal places.

Answer: 0.10 um **[correct]**

Accepted range: 0.10 ± 10%

Feedback/formula:

RC = 31.83 ps, C = epsilon_r epsilon_0 A / W, therefore 50 x epsilon_r epsilon_0 A / W = 31.83 ps.

## Question 6
Consider a Si avalanche photodiode (APD) with breakdown voltage = 150 V, series resistance = 1 ohm and n_m = 2.1.

When biased at 140 V, the dark current is 10 nA. Calculate the gain produced by this APD at a bias of 140 V. Round your answer to 2 decimal places.

Answer: 7.41 **[correct]**

Accepted range: 7.41 ± 10%

Feedback/formula:

M = 1 / [1 - ((V - IR) / Vb)^n]

IR can be ignored if it is much smaller than V.

## Question 7
An Al0.3Ga0.7As photodiode was designed to achieve a quantum efficiency of 37% at a wavelength of 432 nm.

What is the photocurrent produced when incident light, with wavelength 432 nm and optical power 2 mW, is absorbed by the photodiode?

Express your answer in microamperes. Round your answer to 2 decimal places.

Answer: 257.81 uA **[correct]**

Accepted range: 257.81 ± 10%

Feedback/formula:

Photocurrent = Responsivity x Power = eta lambda P / 1.24

## Question 8
1000 photodiodes are required in an optical wireless communication system installed in a shopping mall.

The bitrate is 100 Mb/s, the wavelength is 1550 nm and the average optical power falling on the photodiode is 1 uW.

Which two options are suitable for affordable photodetectors for this application?

A. In0.53Ga0.47As **[correct]**
B. Ge **[correct]**
C. InAs
D. Hg0.8Cd0.2Te
E. InSb

Feedback: Although InAs, InSb and Hg0.8Cd0.2Te can detect long wavelengths, their bandgaps are much smaller than the bandgap needed to detect 1550 nm, where Eg = 1.24 / 1.55 = 0.8 eV. Consequently all three materials have much higher dark currents and are not suitable as low-cost photodetectors for 1550 nm.

## Question 9
An infrared eye-safe LIDAR system is designed to detect an object up to a distance of 1 km.

To achieve high sensitivity, which combination of wavelength and photodiode would you recommend?

A. 1550 nm and InGaAs/InP avalanche photodiode **[correct]**
B. 800 nm and Si phototransistor
C. 600 nm and Si avalanche photodiode
D. 1200 nm and Si avalanche photodiode
E. 700 nm and InGaAs/InP avalanche photodiode

Feedback: Usually wavelength above 900 nm is used. 1200 nm and Si avalanche photodiode is wrong because Si cannot detect 1200 nm. Therefore 1550 nm using InGaAs/InP avalanche photodiode is correct.

## Question 10
An InGaAs double heterojunction photodiode has an InP p-layer, an InGaAs i-layer and an InP n-layer.

Which of the following two advantages are not true?

A. The InP p and n layers increase the breakdown voltage. **[correct: not true]**
B. The InGaAs layer reduces the overall resistance of the photodiode. **[correct: not true]**
C. The wider bandgap InP p and n layers reduce the overall dark current.
D. Only the InGaAs layer absorbs the wavelengths above 1000 nm and determines the quantum efficiency of the photodiode.
E. The InP p and n layers act as transparent window layers in the infrared wavelength of 1300 nm. This reduces recombination loss.

Feedback: All answers are correct except A and B. The breakdown voltage is dependent on the depletion width, which is the InGaAs layer. The InGaAs layer does not reduce the overall resistance; the resistivities of the InP p and n layers control the overall resistance.

## Question 11
A side-injection waveguide photodiode, with wide bandgap p- and n-layers, is used when very high bandwidth is required in optical fibre communication.

Select two statements that are true.

A. The depletion layer is thin but the absorption region can be long to achieve good quantum efficiency. **[correct]**
B. Light is guided within the absorption region which is sandwiched between two wide bandgap semiconductor layers with lower refractive indices. **[correct]**
C. The generation-recombination dark current is reduced because the depletion layer has a wide bandgap.
D. Diffusion dark current is reduced because the depletion region is thin.
E. Waveguide photodiode is cheaper than a vertically illuminated p-i-n photodiode.

Feedback: The correct answers are A and B. Generation-recombination dark current depends on depletion layer thickness and recombination lifetime, and the depletion layer has a narrower bandgap. Diffusion current is reduced due to wider bandgap p and n layers, not because the depletion region is thin. Waveguide photodiodes are more complicated to fabricate, so they are not cheaper.

## Question 12
Low excess avalanche noise factor is produced when:

A. Only one of the carriers can initiate impact ionisation events. **[correct]**
B. A semiconductor with a large bandgap is used.
C. Both electrons and holes can initiate impact ionisation with equal probability.
D. The breakdown voltage is low.
E. The intrinsic carrier concentration is high.

Feedback: Lowest excess noise is obtained when one of the carriers cannot initiate impact ionisation.

## Question 13
CO2 has an absorption band at 4.8 um. Which detector would you recommend to detect CO2 using this absorption band?

A. InSb pn photodiode **[correct]**
B. Hg0.85Cd0.15Te photodiode
C. Si pn photodiode
D. InAs p-i-n photodiode
E. Ge photoconductor
