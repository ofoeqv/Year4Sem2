# H-bridge inverter total BJT conduction losses

## Caption for Word image document
H-bridge inverter total conduction-loss question: a 400 V H-bridge produces a square-wave output across a 123 Ω resistive load. With two BJTs conducting at any time and VCE(sat) = 0.85 V, the total conduction loss of all conducting devices is 5.53 W.

## Where this belongs / folder path
`ta questions/h-bridge/total-bjt-conduction-loss-square-wave-vdc400-r123-vcesat0p85/description.md`

## Question title / short name
H-bridge total BJT conduction losses for square-wave resistive load

## Category
H-bridge

## Subcategory
Semiconductor losses / BJT conduction loss

## Key topic
Calculating total conduction losses in an H-bridge inverter with a resistive load using BJT saturation voltage and load current.

## Full visible question text
The H-bridge inverter shown in the figure below produces a 9 kHz square wave output across the resistive load `R = 123 Ω`. Calculate the total conduction losses (in watts) of all the devices.

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
- Square-wave output frequency: `f = 9 kHz`
- Load resistance: `R = 123 Ω`
- BJT saturation voltage: `VCE(sat) = 0.85 V`
- Load type: resistive

## What the question is asking for
The total average conduction losses of all devices in the H-bridge inverter, in watts.

## Correct answer
`Pcond,total = 5.53 W`

## Method summary
For a resistive load, the current is in phase with the applied square-wave voltage. In a standard bipolar H-bridge square-wave output, two diagonal BJTs conduct at any instant. The diodes do not conduct in the ideal resistive-load conduction path.

Load current magnitude:

`I = Vdc/R = 400/123 = 3.252 A`

Each conducting BJT dissipates:

`Pdevice,on = VCE(sat) × I`

At any instant, two BJTs conduct, so total conduction loss is:

`Pcond,total = 2 × VCE(sat) × I`

Substitute:

`Pcond,total = 2 × 0.85 × 3.252 = 5.528 W`

Rounded to two decimal places:

`Pcond,total = 5.53 W`

The 9 kHz switching frequency is not required for pure conduction loss because the question asks for average conduction losses, not switching losses. Across a full cycle, each BJT conducts for half the time, so summing four devices gives the same result as two conducting devices at any instant.

## Formula / equation source
- Device conduction-loss model for a saturated BJT: `P = VCE(sat) × I` while conducting.
- Circuit reasoning: H-bridge square-wave operation uses two diagonal switches at a time.
- Circuit reasoning: resistive load current magnitude is `I = Vdc/R`.
- Derived total-loss equation: `Pcond,total = 2 VCE(sat) Vdc/R`.

## Must-know concept
In an H-bridge with a resistive load, current follows the commanded voltage. For a bipolar square-wave output, two diagonal switches conduct at a time; the freewheel diodes are not the main conduction path.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded H-bridge circuit/device-parameter screenshots.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic within the archive.

- Manifest check: existing H-bridge entries ask for average load voltage or MOSFET S2 conduction energy loss. This question asks for total BJT conduction losses across all devices.
- Duplicate-logic check: not treated as duplicate logic because the requested element and calculation differ from the archived H-bridge average-voltage question and from the single-MOSFET conduction-energy question.
- Repository search: no exact repository match found for H-bridge total BJT conduction losses, `Vdc = 400 V`, `R = 123 Ω`, `VCE(sat) = 0.85 V`, or square-wave output frequency `9 kHz`.

## Uncertainty
The calculation assumes a standard bipolar square-wave H-bridge output across a purely resistive load, with two BJTs conducting at any instant and no diode conduction in the main current path.
