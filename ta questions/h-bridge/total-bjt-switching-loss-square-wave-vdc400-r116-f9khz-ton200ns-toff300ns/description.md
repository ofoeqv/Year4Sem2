# H-bridge inverter total BJT switching losses

## Caption for Word image document
H-bridge inverter switching-loss question: a 400 V H-bridge produces a 9 kHz square-wave output across a 116 Ω resistive load. With load current I = 400/116 A, two devices switching at each transition, and ton = 200 ns, toff = 300 ns, the total transistor switching loss is 12.41 W.

## Where this belongs / folder path
`ta questions/h-bridge/total-bjt-switching-loss-square-wave-vdc400-r116-f9khz-ton200ns-toff300ns/description.md`

## Question title / short name
H-bridge total BJT switching losses for square-wave resistive load

## Category
H-bridge

## Subcategory
Semiconductor losses / BJT switching loss

## Key topic
Calculating total switching losses in an H-bridge inverter using linear voltage-current overlap during BJT turn-on and turn-off.

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
`Psw,total = 12.41 W`

## Method summary
For a resistive load, the load current magnitude is:

`I = Vdc/R`

`I = 400/116 = 3.448 A`

Using the linear switching-loss approximation for one transistor:

`Eon = 0.5 × Vdc × I × ton`

`Eoff = 0.5 × Vdc × I × toff`

Each transistor turns on once and turns off once per square-wave cycle. There are four transistors, so:

`Psw,total = 4 × 0.5 × Vdc × I × (ton + toff) × f`

Equivalently, at each transition two devices turn off and two devices turn on, and there are two transitions per cycle:

`Psw,total = 2 × Vdc × I × (ton + toff) × f`

Substitute:

`Psw,total = 2 × 400 × 3.448 × (200e−9 + 300e−9) × 9000`

`Psw,total = 12.41 W`

## Formula / equation source
- Formula sheet / semiconductor switching-loss model: `E = 0.5 V I t` for linear voltage-current overlap.
- Circuit reasoning: H-bridge square-wave operation switches diagonal transistor pairs.
- Circuit reasoning: resistive load current magnitude is `I = Vdc/R`.

## Must-know concept
Switching loss depends on how often the transistors switch and on the voltage-current overlap during each transition. In a full H-bridge square wave, all four transistors switch once per output cycle.

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
