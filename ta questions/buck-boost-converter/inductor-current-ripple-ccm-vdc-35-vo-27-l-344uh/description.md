# Buck-boost converter CCM peak-to-peak inductor current ripple

## Caption for Word image document
Buck-boost converter CCM inductor-ripple question: Vdc = 35 V, |Vo| = 27 V, fpwm = 50 kHz, L = 344 µH, and C = 47 µF; using the CCM buck-boost duty ratio and Mode 1 inductor ramp gives a peak-to-peak inductor current ripple of ΔIL = 0.89 A.

## Where this belongs / folder path
`ta questions/buck-boost-converter/inductor-current-ripple-ccm-vdc-35-vo-27-l-344uh/description.md`

## Question title / short name
Buck-boost CCM inductor ripple, Vdc 35 V and Vo 27 V

## Category
Buck-boost converter

## Subcategory
CCM inductor-current ripple

## Key topic
Peak-to-peak inductor current ripple in an inverting buck-boost converter operating in continuous current conduction mode.

## Full visible question text
Calculate the peak-to-peak inductor current ripple (in amperes) of a Buck-boost converter assuming it operates in continuous current conduction mode.

Circuit parameters are: Input voltage Vdc = 35 V, output voltage Vo = 27 V, PWM frequency fpwm = 50 kHz, inductor value 344 µH and capacitor value C = 47µF.

Please specify your answer in units of A to 2 decimal places.

## Given values
- Input voltage: `Vdc = 35 V`
- Output voltage magnitude: `Vo = 27 V`
- PWM frequency: `fpwm = 50 kHz`
- Inductor: `L = 344 µH`
- Capacitor: `C = 47 µF`
- Operating mode: `CCM`

## What the question is asking for
The peak-to-peak inductor current ripple `ΔIL` in amperes.

## Correct answer
`ΔIL = 0.89 A`

## Method summary
For an inverting buck-boost converter in CCM, the output-voltage relation is:

`|Vo| = Vdc × d / (1 − d)`

so:

`d = |Vo| / (Vdc + |Vo|) = 27 / (35 + 27) = 0.4355`

During Mode 1, the switch is on, the diode is off, and the inductor has approximately `Vdc` across it. Therefore:

`ΔIL = (Vdc / L) × ton`

with:

`ton = d / fpwm`

Combining:

`ΔIL = Vdc × d / (L × fpwm)`

Substitute the values:

`ΔIL = 35 × 0.4355 / (344e−6 × 50e3) = 0.886 A ≈ 0.89 A`

The capacitor value is not required for the inductor ripple calculation.

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: in buck-boost CCM Mode 1, the switch is on and `vL = Vdc`, so the inductor current rises linearly.
- Circuit reasoning / buck-boost CCM volt-second balance: `|Vo| = Vdc d/(1−d)` for magnitude form, equivalent to signed `Vo = −Vdc d/(1−d)`.

## Must-know concept
In buck-boost CCM, inductor ripple is set by the inductor voltage during the ON interval and the ON time. The output capacitor affects output voltage ripple, not the inductor current ripple calculation here.

## Date archived
2026-05-29

## Original image filename
`image.png`

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new similar-not-duplicate.

- Manifest check: a similar archived buck-boost CCM inductor-current ripple question exists, but it uses `Vdc = 42 V`, `Vo = 14 V`, `fpwm = 50 kHz`, and `L = 462 µH`, with answer `0.45 A`. This new question has different values and a different correct answer.
- Repository search: no exact match found for the combination `Vdc = 35 V`, `Vo = 27 V`, `fpwm = 50 kHz`, `L = 344 µH`, and requested `ΔIL`.
- Decision: archive as a new question.

## Uncertainty
No visible value uncertainty. The prompt clearly gives `Vdc = 35 V`, `Vo = 27 V`, `fpwm = 50 kHz`, `L = 344 µH`, and `C = 47 µF`.
