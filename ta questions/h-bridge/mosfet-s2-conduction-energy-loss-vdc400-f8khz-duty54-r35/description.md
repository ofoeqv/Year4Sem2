# H-bridge MOSFET S2 conduction energy loss

## Caption for Word image document
H-bridge MOSFET conduction-energy question: a 400 V H-bridge drives a 35 Ω resistive load at 8 kHz with S1 duty cycle 54%; MOSFET S2 conducts during the complementary interval, 46%, and with rDS(on) = 25 mΩ the conduction energy loss in S2 is 0.19 mJ per switching period.

## Where this belongs / folder path
`ta questions/h-bridge/mosfet-s2-conduction-energy-loss-vdc400-f8khz-duty54-r35/description.md`

## Question title / short name
H-bridge MOSFET S2 conduction energy loss

## Category
H-bridge

## Subcategory
Semiconductor losses / MOSFET conduction energy

## Key topic
Calculating conduction energy loss in one MOSFET of an H-bridge from load current, MOSFET on-resistance, complementary switch duty, and switching period.

## Full visible question text
A H-bridge converter employing four MOSFET devices and four diodes is connected to a dc source of 400 V and operates at 8 kHz. The duty cycle of switch S1 is 54 % and the load is R = 35 Ω. The circuit diagram and device parameters are given below.

Determine the conduction energy losses in MOSFET S2.

Device parameters shown:

MOSFET:
- `Imax = 25 A`
- `Vmax = 300 V`
- `rds(on) = 25 mΩ`
- `ton = 100 ns`
- `toff = 200 ns`

Diodes:
- `Vfwd = 0.25 V`
- `Imax = 25 A`
- `Vmax = 300 V`
- `rf = 5 mΩ`

## Given values
- DC source: `Vdc = 400 V`
- Switching frequency: `f = 8 kHz`
- Switching period: `T = 1/f = 125 µs`
- Duty cycle of S1: `d = 54% = 0.54`
- Complementary conduction fraction for S2: `1 − d = 0.46`
- Load resistance: `R = 35 Ω`
- MOSFET on-resistance: `rDS(on) = 25 mΩ = 0.025 Ω`

## What the question is asking for
The conduction energy loss in MOSFET `S2`, in millijoules.

## Correct answer
`Econd,S2 = 0.19 mJ`

## Method summary
For a resistive load in a bipolar H-bridge switching pattern, the diagonal pair `S1/S4` conducts during the `S1` duty interval and the opposite diagonal pair `S2/S3` conducts during the complementary interval. Therefore, `S2` conducts for:

`(1 − d)T`

The load current magnitude during conduction is:

`I = Vdc/R = 400/35 = 11.43 A`

The MOSFET conduction power while it is on is:

`Pcond,on = I² rDS(on)`

`Pcond,on = 11.43² × 0.025 = 3.27 W`

The energy dissipated by `S2` over one switching period is:

`Econd,S2 = Pcond,on × (1 − d)T`

`Econd,S2 = 3.27 × 0.46 × 125 µs = 0.0001878 J`

Convert to millijoules:

`Econd,S2 = 0.1878 mJ ≈ 0.19 mJ`

## Formula / equation source
- Device conduction-loss model: `P = I² rDS(on)` for MOSFET conduction.
- Circuit reasoning: H-bridge resistive load current magnitude is `I = Vdc/R` when a diagonal switch pair applies the DC bus across the load.
- Circuit reasoning: if `S1` has duty `d`, then the complementary diagonal containing `S2` conducts for `1 − d` in bipolar operation.
- Derived conduction-energy equation: `Econd,S2 = (Vdc/R)² rDS(on) (1−d) / f`.

## Must-know concept
Conduction energy is on-state conduction power multiplied by the time the device conducts. For `S2`, use the complementary duty interval, not the `S1` duty interval.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded H-bridge circuit/device-parameter screenshots.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic within the archive.

- Manifest check: an existing H-bridge question asks for average load voltage from S1 duty cycle, but it does not ask for MOSFET conduction energy loss.
- Duplicate-logic check: no archived question currently asks for conduction energy loss of a specific MOSFET in an H-bridge using `I²rDS(on)` and device conduction time.
- Repository search: no exact repository match found for H-bridge MOSFET S2 conduction energy loss, `Vdc = 400 V`, `f = 8 kHz`, `d = 54%`, `R = 35 Ω`, or `rDS(on) = 25 mΩ`.

## Uncertainty
The calculation assumes standard bipolar H-bridge switching where `S1/S4` conduct for duty `d` and `S2/S3` conduct for `1−d`. The prompt gives `S1` duty cycle only, so this complementary-switching assumption is required.
