# Buck converter boundary CCM/DCM average input current

## Caption for Word image document
Buck converter boundary-conduction average-input-current question: with Vdc = 29 V, Vo = 15 V, fpwm = 50 kHz, and L = 16 µH, the boundary inductor ripple gives Io = 4.53 A and the average input current is Is,avg = δIo = 2.34 A.

## Where this belongs / folder path
`ta questions/buck-converters/boundary-ccm-dcm-average-input-current-vdc29-vo15-l16uh-f50khz/description.md`

## Question title / short name
Buck boundary CCM/DCM average input current

## Category
Buck converters

## Subcategory
Boundary conduction / average input current

## Key topic
Finding the average input current of a buck converter operating at the boundary between continuous and discontinuous conduction modes.

## Full visible question text
Question 2. Calculate the average input current (in amperes) to the Buck dc to dc power converter. The converter works at the boundary between the continuous and discontinuous modes with the following parameters:

Input voltage Vdc = 29 V, output voltage Vo = 15 V, PWM frequency fpwm = 50 kHz, inductor value L = 16 µH and capacitor value C = 200 µF.

Please specify your answer in units of A to 2 decimal places.

## Given values
- Converter: Buck converter
- Input voltage: `Vdc = 29 V`
- Output voltage: `Vo = 15 V`
- Switching frequency: `fpwm = 50 kHz`
- Inductor: `L = 16 µH`
- Capacitor: `C = 200 µF`
- Operating condition: boundary between CCM and DCM

## What the question is asking for
The average input current to the buck converter, in amperes.

## Correct answer
`Is,avg = 2.34 A`

## Method summary
For an ideal buck converter:

`δ = Vo/Vdc`

`δ = 15/29 = 0.5172`

At the CCM/DCM boundary, the inductor current just touches zero. The inductor current is triangular, so:

`Io = IL,avg = ΔIL/2`

During the switch-on interval, the buck inductor voltage is:

`vL = Vdc − Vo`

Using `vL = L diL/dt`:

`ΔIL = (Vdc − Vo)δ/(L fpwm)`

Substitute:

`ΔIL = (29 − 15)(15/29)/(16e−6 × 50e3) = 9.05 A`

So:

`Io = ΔIL/2 = 4.53 A`

The input current flows only during the switch-on interval. For an ideal buck converter:

`Is,avg = δ Io`

`Is,avg = 0.5172 × 4.53 = 2.34 A`

The capacitor value is not required for this average input-current calculation.

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: ideal buck duty relation `Vo = δVdc`.
- Circuit reasoning: in switch-on mode, buck inductor voltage is `Vdc − Vo`.
- Boundary condition: at CCM/DCM boundary, `Io = ΔIL/2`.
- Circuit reasoning / ideal power balance: average input current for buck is `Is,avg = δIo`.

## Must-know concept
At the CCM/DCM boundary, the inductor current is a triangle that just reaches zero. The source only supplies current during switch-on, so the average input current is the output/inductor average current multiplied by the duty ratio.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded buck converter screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a distinct buck boundary-conduction category question.

- Repository search found no exact existing archive entry for this specific average-input-current question.
- Similar existing entry: buck converter boundary CCM/DCM inductor value. That entry asks for `L`, while this question asks for average input current and uses the given `L` to infer boundary current.
- Decision: archive as distinct because the requested quantity and revision skill are different, even though both use boundary-conduction reasoning.

## Uncertainty
No visible value uncertainty. The prompt clearly gives `Vdc = 29 V`, `Vo = 15 V`, `fpwm = 50 kHz`, `L = 16 µH`, and `C = 200 µF`.
