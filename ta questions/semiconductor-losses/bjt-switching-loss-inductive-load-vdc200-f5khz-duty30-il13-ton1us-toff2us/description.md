# BJT switch switching losses with inductive load and freewheeling diode

## Caption for Word image document
BJT inductive-load switching-loss question: using the inductive-load switching-energy approximation Esw = (Vdc IL/2)tsw for turn-on and turn-off, the switching loss is Psw = (Vdc IL/2)(ton + toff)fpwm = 19.50 W.

## Where this belongs / folder path
`ta questions/semiconductor-losses/bjt-switching-loss-inductive-load-vdc200-f5khz-duty30-il13-ton1us-toff2us/description.md`

## Question title / short name
BJT switching loss for inductive load with freewheeling diode

## Category
Semiconductor losses

## Subcategory
BJT switching loss / inductive load

## Key topic
Calculating BJT switching power loss using switching-energy overlap for an inductive-load switch.

## Full visible question text
A BJT switch operating at 5 kHz switches an inductive load across a dc supply `Vdc` of 200 V with a duty cycle of 30 %. The inductive load is modelled by a current source `IL` of 13 A. A freewheeling diode is connected in parallel with the load. The circuit schematic and device characteristics are included below.

Calculate the switching losses, in watts, of the BJT switch.

Device characteristics visible:
- BJT: `Imax = 25 A`
- BJT: `Vmax = 300 V`
- BJT: `VCE(sat) = 0.7 V`
- BJT: `ton = 1 µs`
- BJT: `toff = 2 µs`
- Diode: `Vfwd = 0.3 V`
- Diode: `Imax = 25 A`
- Diode: `Vmax = 300 V`
- Diode: `Rf = 10 mΩ`

## Given values
- Supply voltage: `Vdc = 200 V`
- PWM frequency: `fpwm = 5 kHz`
- Duty cycle: `δ = 30 %`
- Load current: `IL = 13 A`
- BJT turn-on time: `ton = 1 µs`
- BJT turn-off time: `toff = 2 µs`

## What the question is asking for
The BJT switching losses in watts.

## Correct answer
`19.50 W`

## Method summary
For an inductive-load switch, the switching energy is approximated by the triangular overlap of device voltage and current:

`Esw = (Vdc IL / 2) tsw`

Total switching energy per cycle includes both turn-on and turn-off:

`Esw,total = (Vdc IL / 2)(ton + toff)`

Switching power loss is switching energy per cycle multiplied by switching frequency:

`Psw = (Vdc IL / 2)(ton + toff)fpwm`

Substitute values:

`Psw = (200 × 13 / 2)(1 µs + 2 µs)(5000)`

`Psw = 1300 × 3×10^-6 × 5000`

`Psw = 19.50 W`

## Formula / equation source
- Formula sheet: switching energy loss for inductive load, `Esw = (Vdc IS/2)tsw`.
- Circuit reasoning: the BJT switches an inductive load modelled as a nearly constant current source, so use the inductive-load switching-loss expression.

## Must-know concept
For switching loss, use the voltage-current overlap during transitions. Duty cycle and `VCE(sat)` are for conduction loss, not switching loss, unless the question asks for total device loss.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded schematic/device-characteristics screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a new semiconductor-loss question.

- Repository search found no exact existing archive entry for a single BJT inductive-load switching-loss calculation with `Vdc = 200 V`, `IL = 13 A`, `fpwm = 5 kHz`, `ton = 1 µs`, and `toff = 2 µs`.
- Existing related entries cover freewheeling diode conduction loss and H-bridge BJT conduction/switching losses, but not this single-switch BJT inductive-load switching-loss calculation.
- Decision: archive as a distinct semiconductor-loss calculation type.

## Uncertainty
No visible value uncertainty. The answer assumes the question asks for switching loss of the BJT switch only, not total loss including conduction loss.
