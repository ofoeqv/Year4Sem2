# H-bridge inverter total BJT switching losses

## Caption for Word image document
H-bridge inverter switching-loss question: a 400 V H-bridge produces a 9 kHz square-wave output across a 116 Ω resistive load. With load current I = 400/116 A and BJT switching times ton = 200 ns, toff = 300 ns, the resistive-load switching-loss factor is 1/6 per switching event, giving total transistor switching loss Psw,total = 4.14 W.

## Where this belongs / folder path
`ta questions/h-bridge/total-bjt-switching-loss-square-wave-vdc400-r116-f9khz-ton200ns-toff300ns/description.md`

## Question title / short name
H-bridge total BJT switching losses for square-wave resistive load

## Category
H-bridge

## Subcategory
Semiconductor losses / BJT switching loss / resistive load

## Key topic
Calculating total switching losses in an H-bridge inverter with a resistive load using the resistive switching-loss overlap factor.

## Full visible question text
The H-bridge inverter shown in the figure below produces a `9 kHz` square wave output across the resistive load `R = 116 Ω`. Calculate the combined switching losses (in watts) in the transistors.

Device parameters shown:

BJT:
- `Imax = 25 A`
- `Vmax = 500 V`
- `VCE(sat) = 0.85 V`
- `ton = 200 ns`
- `toff = 300 ns`

Diodes:
- `Vfwd = 0.3 V`
- `Imax = 25 A`
- `Vmax = 500 V`
- `Rf = 10 mΩ`

Please specify your answer in units of W to 2 decimal places.

## Given values
- DC link voltage: `Vdc = 400 V`
- Square-wave frequency: `f = 9 kHz`
- Load resistance: `R = 116 Ω`
- BJT turn-on time: `ton = 200 ns`
- BJT turn-off time: `toff = 300 ns`
- Load type: resistive

## What the question is asking for
The total average switching losses in the H-bridge transistors, in watts.

## Correct answer
`Psw,total = 4.14 W`

## Method summary
For a resistive load, the load current is in phase with the output voltage and its magnitude is:

`I = Vdc/R`

`I = 400/116 = 3.448 A`

For a resistive-load switching transition, the ELE336 formula-sheet switching-energy approximation uses the factor `1/6`, not `1/2`:

`Esw,resistive = (1/6) × Vdc × I × tsw`

For one BJT over one full output cycle:

`Psw,1 = (1/6) × Vdc × I × (ton + toff) × f`

There are four BJTs in the H-bridge, so:

`Psw,total = 4 × (1/6) × Vdc × I × (ton + toff) × f`

Substitute:

`Psw,total = (4/6) × 400 × 3.448 × (200e−9 + 300e−9) × 9000`

`Psw,total = 4.14 W`

## Correction note
The original archived calculation incorrectly used the inductive/current-source switching-loss factor `1/2`, giving `12.41 W`. That was corrected because the prompt explicitly states a resistive load. For the stated resistive-load H-bridge case, the correct factor is `1/6`, giving `4.14 W`.

## Formula / equation source
- Formula sheet: resistive-load switching-energy expression uses the `1/6` overlap factor.
- Formula sheet contrast: inductive/current-source switching-energy expression uses the `1/2` overlap factor.
- H-bridge circuit reasoning: for a resistive square-wave load, `I = Vdc/R` and current is in phase with voltage.

## Must-know concept
Resistive switching loss is smaller than inductive/current-source switching loss because voltage and current change together during the transition. Use the `1/6` factor for resistive load switching and the `1/2` factor for inductive/current-source switching.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded H-bridge circuit/device-parameter screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived question.

## Duplicate-check result
Status: new H-bridge semiconductor-loss category question.

- Repository search found no exact existing archive entry for H-bridge total BJT switching losses.
- Similar existing H-bridge entries include average load voltage, MOSFET S2 conduction energy, and total BJT conduction losses. This question asks for total BJT switching losses, so it is a distinct requested quantity and method.

## Uncertainty
No visible value uncertainty. The prompt clearly gives `Vdc = 400 V`, `R = 116 Ω`, `f = 9 kHz`, `ton = 200 ns`, and `toff = 300 ns`.
