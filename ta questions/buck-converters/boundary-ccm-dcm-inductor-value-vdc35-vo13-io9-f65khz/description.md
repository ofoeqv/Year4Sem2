# Buck converter boundary CCM/DCM inductor value

## Caption for Word image document
Buck converter boundary-conduction inductor-sizing question: with Vdc = 35 V, Vo = 13 V, Io = 9 A, and fpwm = 65 kHz, the boundary condition ΔIL = 2Io gives the required inductor value L = 6.98 µH.

## Where this belongs / folder path
`ta questions/buck-converters/boundary-ccm-dcm-inductor-value-vdc35-vo13-io9-f65khz/description.md`

## Question title / short name
Buck boundary CCM/DCM inductor value

## Category
Buck converters

## Subcategory
Boundary conduction / CCM-DCM boundary inductor sizing

## Key topic
Finding the inductor value that places a buck converter at the boundary between continuous and discontinuous conduction modes.

## Full visible question text
Calculate the inductor value (in µH) of a Buck converter designed to operate at the boundary between the continuous and discontinuous modes with the following specification: Input voltage Vdc = 35 V, output current Io = 9 A, output voltage Vo = 13 V, switching frequency fpwm = 65 kHz and capacitor value C = 100µF.

## Given values
- Converter: Buck converter
- Input voltage: `Vdc = 35 V`
- Output voltage: `Vo = 13 V`
- Output current: `Io = 9 A`
- Switching frequency: `fpwm = 65 kHz`
- Capacitor: `C = 100 µF`
- Operating condition: boundary between CCM and DCM

## What the question is asking for
The inductor value `L` in microhenries that makes the buck converter operate at the CCM/DCM boundary.

## Correct answer
`L = 6.98 µH`

## Method summary
For an ideal buck converter:

`δ = Vo/Vdc`

`δ = 13/35 = 0.3714`

At the boundary between CCM and DCM, the inductor current just reaches zero at the end of the switching period. Therefore the peak-to-peak inductor current ripple is:

`ΔIL = 2Io`

During switch on-time, the buck inductor voltage is:

`vL = Vdc − Vo`

Using `vL = L diL/dt`:

`ΔIL = (Vdc − Vo) δ / (L fpwm)`

Rearrange for `L`:

`L = (Vdc − Vo) δ / (2Io fpwm)`

Substitute:

`L = (35 − 13)(13/35) / (2 × 9 × 65000)`

`L = 6.984e−6 H = 6.98 µH`

The capacitor value is not required for this boundary-inductor calculation.

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: ideal buck duty relation `Vo = δVdc`.
- Circuit reasoning: in switch-on mode, buck inductor voltage is `Vdc − Vo`.
- Boundary condition: at CCM/DCM boundary, `ΔIL = 2Io`.

## Must-know concept
At the CCM/DCM boundary, the triangular inductor current ripple is just large enough for the minimum inductor current to touch zero. That is why the ripple magnitude equals twice the average output/load current.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded buck converter screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived under buck converters as requested by user.

- Repository search found no exact existing archive entry for this specific buck boundary CCM/DCM inductor-sizing question.
- Earlier discussion treated this as a duplicate-logic candidate because it is a standard boundary-inductor sizing method, but the user explicitly requested that it be archived under buck converters.
- This is now stored as a buck converter boundary-conduction category question.

## Uncertainty
No visible value uncertainty. The prompt clearly gives `Vdc = 35 V`, `Vo = 13 V`, `Io = 9 A`, `fpwm = 65 kHz`, and `C = 100 µF`.
