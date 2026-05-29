# Buck-boost CCM inductor current ripple

## Question title / short name
Buck-boost converter CCM peak-to-peak inductor current ripple

## Category
buck-boost-converter

## Subcategory
ccm-inductor-current-ripple

## Key topic
Inductor current ripple in an inverting buck-boost converter operating in continuous current conduction mode.

## Full visible question text
Calculate the peak-to-peak inductor current ripple (in amperes) of a Buck-boost converter assuming it operates in continuous current conduction mode.

Circuit parameters are: Input voltage Vdc = 42 V, output voltage Vo = 14 V, PWM frequency fpwm = 50 kHz, inductor value 462 μH and capacitor value C = 47 μF. Please specify your answer in units of A to 2 decimal places.

## Given values
- Input voltage, Vdc = 42 V
- Output voltage, Vo = 14 V (treated as output-voltage magnitude for the inverting buck-boost)
- PWM frequency, fpwm = 50 kHz
- Inductor, L = 462 μH
- Capacitor, C = 47 μF
- Operating mode: continuous current conduction mode (CCM)

## What the question is asking for
Calculate the peak-to-peak inductor current ripple, ΔIL, in amperes, to 2 decimal places.

## Correct answer
ΔIL = 0.45 A

## Method summary
For an inverting buck-boost converter in CCM, use the voltage conversion relation with the output-voltage magnitude:

D = |Vo| / (Vdc + |Vo|) = 14 / (42 + 14) = 0.25

The switch on-time is:

ton = D / fpwm = 0.25 / 50 kHz = 5 μs

During switch-on, the inductor sees vL = Vdc, so:

ΔIL = (Vdc / L) ton = (42 / 462 μH)(5 μs) = 0.4545 A ≈ 0.45 A

Cross-check during switch-off:

toff = (1 - D) / fpwm = 15 μs

ΔIL = (|Vo| / L) toff = (14 / 462 μH)(15 μs) = 0.4545 A

## Formula / equation source
- Formula-sheet equation: inductor voltage-current law, vL = L diL/dt.
- Circuit reasoning: in buck-boost CCM, vL = Vdc during switch-on and vL = -|Vo| during diode conduction.
- Derived by volt-second balance: Vdc·ton = |Vo|·toff, giving D = |Vo| / (Vdc + |Vo|).

## Date archived
2026-05-29

## Original image filename
image.png

## Image metadata
- Stored image path: `ta questions/buck-boost-converter/inductor-current-ripple-ccm-vdc-42-vo-14-l-462uh/question.png`
- SHA-256: `1bf97b24540470b5b13cc2e886def27632337a7911f6f545bce55c37d8386319`
- Size: 484 × 203 px

## Duplicate-check result
New question. No duplicate was found in the existing manifest, and repository text search found no matching stored question/values before archiving.
