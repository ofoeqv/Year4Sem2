# Turn-on snubber inductor for MOSFET drain-current rise time

## Caption for Word image document
Turn-on snubber sizing question: MOSFET switch with inductive load, Vdc = 187 V, fpwm = 5 kHz, duty d = 30 %, and load current IL = 5 A; the series snubber inductor Ls is chosen so the MOSFET drain current rises to IL in 1 µs, giving Ls = 37.40 µH.

## Where this belongs / folder path
`ta questions/snubbers/turn-on-snubber-inductor-vdc-187-fpwm-5khz-il-5a-trise-1us/description.md`

## Question title / short name
Turn-on snubber inductor from drain-current rise time

## Category
Snubbers

## Subcategory
Turn-on snubber / inductor sizing

## Key topic
Using a series snubber inductor to control MOSFET drain-current rise during turn-on.

## Full visible question text
A MOSFET switch operating PWM frequency 5 kHz switches an inductive load across a dc supply Vdc of 187 V with a duty cycle of d = 30 %. A turn-on snubber circuit featuring an inductor Ls, a resistor Rs and a diode Ds is used to control the fall-time of the MOSFET’s drain-source voltage. Assuming the MOSFET turn-on response is dominated by the snubber circuit, what value of Ls is required to achieve a drain current rise time of 1µs if the load current is IL is 5 A?

Please specify your answer in units of µH to 2 decimal places.

## Given values
- DC supply voltage: `Vdc = 187 V`
- PWM frequency: `fpwm = 5 kHz`
- Duty cycle: `d = 30 %`
- Load current: `IL = 5 A`
- Required MOSFET drain-current rise time: `tr = 1 µs`
- Snubber elements: `Ls`, `Rs`, `Ds`

## What the question is asking for
The required turn-on snubber inductance `Ls`, in microhenries, to make the MOSFET drain current rise to the load current in `1 µs`.

## Correct answer
`Ls = 37.40 µH`

## Method summary
The snubber inductor limits the drain-current slew rate during MOSFET turn-on. Assuming the snubber dominates the switching transient, the inductor voltage is approximately the DC link voltage while the current rises from `0 A` to `IL`.

Using `vL = L di/dt`:

`Ls = Vdc × tr / IL`

Substitute the values:

`Ls = 187 × 1e-6 / 5 = 37.4e-6 H = 37.40 µH`

The PWM frequency and duty cycle are contextual operating conditions here; they are not needed for the inductor rise-time calculation.

## Formula / equation source
- Direct formula-sheet equation: `vL = L diL/dt`.
- Circuit reasoning: during the turn-on transient, `Ls` is treated as having approximately `Vdc` across it while the drain current ramps from `0` to `IL`.
- Derived sizing equation: `Ls = Vdc tr / IL`.

## Must-know concept
A turn-on snubber inductor slows the rise of MOSFET current. Bigger `Ls` means a slower current ramp because the same voltage produces a smaller `di/dt`.

## Date archived
2026-05-29

## Original image filename
`image.png`

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new question.

- Manifest check: no exact existing entry for a turn-on snubber inductor with `Vdc = 187 V`, `IL = 5 A`, and `tr = 1 µs`.
- Similar existing item: a snubber entry exists for a turn-off snubber resistor calculation, but it asks for `Rs`, uses different values, and is not the same question.
- Repository search: no exact match found for the question wording, values, or requested quantity.

## Uncertainty
No visible value uncertainty. The image and typed prompt clearly show `Vdc = 187 V`, `fpwm = 5 kHz`, `d = 30 %`, `IL = 5 A`, and rise time `1 µs`.
