# Turn-on snubber peak MOSFET drain-source voltage at turn-off

## Caption for Word image document
Turn-on snubber peak-voltage question: a MOSFET chopper uses Ls = 10 µH and Rs = 38 Ω with Vdc = 111 V and load current IL = 9 A. At turn-off, Ds conducts and Rs produces an extra ILRs voltage, so the peak MOSFET drain-source voltage is VDS,peak = Vdc + ILRs = 453.00 V.

## Where this belongs / folder path
`ta questions/snubbers/turn-on-snubber-peak-vds-turnoff-vdc111-il9-rs38-ls10uh/description.md`

## Question title / short name
Turn-on snubber peak VDS during turn-off

## Category
Snubbers

## Subcategory
Turn-on snubber / MOSFET voltage stress

## Key topic
Finding the peak drain-source voltage experienced by the MOSFET during turn-off when the turn-on snubber reset path conducts through Rs.

## Full visible question text
A MOSFET switch operating at 5 kHz switches an inductive load across a dc supply `Vdc = 111 V` with a duty cycle of `40 %`. A turn-on snubber circuit featuring an inductor `Ls = 10 µH`, a resistor `Rs = 38 Ω` and a diode `Ds` is used to control the fall-time of the MOSFET's drain-source voltage. If the inductor current is `IL = 9 A`, what is peak drain source voltage experienced by the MOSFET during turn-off?

Please specify your answer in units of V to 2 decimal places.

## Given values
- Converter/switch circuit: MOSFET chopper with turn-on snubber
- DC supply voltage: `Vdc = 111 V`
- PWM frequency: `fpwm = 5 kHz`
- Duty cycle: `d = 40 %`
- Snubber inductor: `Ls = 10 µH`
- Snubber resistor: `Rs = 38 Ω`
- Snubber diode: `Ds`
- Load/inductor current: `IL = 9 A`

## What the question is asking for
The peak drain-source voltage `VDS,peak` experienced by the MOSFET during turn-off, in volts.

## Correct answer
`VDS,peak = 453.00 V`

## Method summary
For a turn-on snubber, at the instant of MOSFET turn-off the snubber diode `Ds` conducts and the snubber inductor current is reset through the snubber resistor `Rs`.

The resistor produces an extra voltage:

`VRs = IL Rs`

This voltage adds to the DC supply voltage across the MOSFET:

`VDS,peak = Vdc + IL Rs`

Substitute:

`VDS,peak = 111 + (9 × 38)`

`VDS,peak = 111 + 342 = 453 V`

Therefore:

`VDS,peak = 453.00 V`

The values `fpwm`, duty cycle, and `Ls` are not needed once `Rs` and `IL` are already given. They are relevant to the reset/design of the snubber, but not to this peak-voltage calculation.

## Formula / equation source
- Circuit reasoning from turn-on snubber operation: at MOSFET turn-off, `Ds` conducts and `ILRs` is generated across `Rs`.
- Derived voltage-stress equation: `VDS,peak = Vdc + ILRs`.
- Tutorial sheet 3 solutions use the same principle: with the snubber installed, at turn-off `Ds` conducts and the MOSFET voltage rating must include `ILRs + Vdc`.

## Must-know concept
A turn-on snubber reduces turn-on stress, but during turn-off its reset resistor creates an extra overvoltage. The MOSFET must block the DC supply plus the `ILRs` reset voltage.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded circuit screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived question.

## Duplicate-check result
Status: new snubber category question.

- Repository search found no exact existing archive entry for turn-on snubber peak MOSFET drain-source voltage at turn-off.
- Similar snubber entries exist for turn-on snubber inductor sizing and turn-off snubber resistor/capacitor sizing, but this question asks for MOSFET voltage stress using `Vdc + ILRs`.
- Decision: archived under snubbers as a distinct turn-on snubber voltage-stress question.

## Uncertainty
No visible value uncertainty. The prompt clearly gives `Vdc = 111 V`, `Rs = 38 Ω`, and `IL = 9 A`.
