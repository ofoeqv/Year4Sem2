# Freewheeling diode conduction loss in BJT inductive-load switch

## Caption for Word image document
Freewheeling diode conduction-loss question: a BJT switches an 8 A inductive load from a 200 V DC supply at 5 kHz with duty cycle d = 41%; the freewheeling diode conducts during the off interval, so using V_fwd = 0.3 V and R_fwd = 10 mΩ gives an average diode conduction loss of 1.79 W.

## Where this belongs / folder path
`ta questions/semiconductor-losses/freewheeling-diode-conduction-loss-bjt-vdc200-duty41-il8/description.md`

## Question title / short name
Freewheeling diode conduction loss for BJT inductive-load switch

## Category
Semiconductor losses

## Subcategory
Freewheeling diode / conduction loss

## Key topic
Calculating the average conduction power loss of a freewheeling diode using its forward voltage, forward resistance, load current, and conduction duty interval.

## Full visible question text
A BJT switch operating at 5 kHz switches an inductive load across a dc supply Vdc of 200 V with a duty cycle of 41 %. The inductive load is modelled by a current source IL of 8 A. A freewheeling diode is connected in parallel with the load. The circuit schematic and devices characteristics are included below.

Calculate the conduction losses (in watts) of the freewheeling diode.

Device characteristics shown:

BJT:
- `Imax = 25 A`
- `Vmax = 300 V`
- `VCE(sat) = 0.7 V`
- `ton = 1 µs`
- `toff = 2 µs`

Diode:
- `Vfwd = 0.3 V`
- `Imax = 25 A`
- `Vmax = 300 V`
- `Rfwd = 10 mΩ`

## Given values
- Switching frequency: `f = 5 kHz`
- DC supply: `Vdc = 200 V`
- Duty cycle of BJT on-time: `d = 41% = 0.41`
- Load current: `IL = 8 A`
- Freewheeling diode forward voltage: `Vfwd = 0.3 V`
- Freewheeling diode forward resistance: `Rfwd = 10 mΩ = 0.01 Ω`

## What the question is asking for
The average conduction loss of the freewheeling diode in watts.

## Correct answer
`P_D,cond = 1.79 W`

## Method summary
The freewheeling diode conducts when the BJT is off, so the diode conduction fraction is:

`1 − d = 1 − 0.41 = 0.59`

The instantaneous diode conduction loss while carrying the load current is:

`P_D,on = Vfwd IL + Rfwd IL^2`

Substitute the diode parameters:

`P_D,on = 0.3 × 8 + 0.01 × 8^2`

`P_D,on = 2.4 + 0.64 = 3.04 W`

Average over the full switching period:

`P_D,cond = (1 − d) × P_D,on`

`P_D,cond = 0.59 × 3.04 = 1.7936 W`

Rounded to two decimal places:

`P_D,cond = 1.79 W`

The switching frequency does not affect this conduction-loss calculation directly because the duty ratio already gives the fraction of time the diode conducts.

## Formula / equation source
- Device conduction-loss model: `P = VI + I^2R` during conduction.
- Circuit reasoning: in an inductive-load BJT switch with a freewheeling diode, the diode conducts during the transistor off-time, so diode duty fraction is `1 − d`.
- Derived average-loss equation: `P_D,cond = (1 − d)(Vfwd IL + Rfwd IL^2)`.

## Must-know concept
The freewheeling diode does not conduct while the BJT is on. It conducts during the off interval to keep the inductive load current flowing, so its average conduction loss is multiplied by `1 − d`, not by `d`.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded circuit/device-characteristics screenshots.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic within the archive.

- Manifest check: no existing archived freewheeling-diode conduction-loss question found.
- Duplicate-logic check: no archived question currently asks for diode conduction loss using diode forward voltage/resistance, load current, and transistor off-duty interval.
- Repository search: no exact repository match found for freewheeling diode conduction losses, `Vfwd = 0.3 V`, `Rfwd = 10 mΩ`, `IL = 8 A`, duty `41%`, or `Vdc = 200 V`.

## Uncertainty
No visible value uncertainty. The typed prompt clearly gives `f = 5 kHz`, `Vdc = 200 V`, `d = 41%`, and `IL = 8 A`; the image clearly shows diode values `Vfwd = 0.3 V` and `Rfwd = 10 mΩ`.
