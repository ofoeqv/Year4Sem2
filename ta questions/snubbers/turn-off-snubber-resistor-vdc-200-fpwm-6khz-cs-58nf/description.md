# Turn-off snubber resistor sizing

## Caption for your Word image document
Turn-off snubber sizing case study for a MOSFET chopper with inductive-load current source: the circuit uses a snubber capacitor Cs, snubber diode Ds, and discharge resistor Rs to limit the MOSFET drain-source voltage rise at turn-off; here Vdc = 200 V, fpwm = 6 kHz, Cs = 58 nF, and the worst-case minimum duty cycle is 10%.

## Question title / short name
Turn-off snubber resistor from minimum duty cycle

## Category
snubbers

## Subcategory
turn-off-snubber / resistor-sizing

## Key topic
Sizing the snubber discharge resistor Rs so that the snubber capacitor Cs discharges during the MOSFET on-time.

## Full visible question text
The circuit below shows a MOSFET switch operating with a turn-off snubber operating from a DC supply voltage Vdc = 200 V. The circuit operates using PWM with a frequency of fpwm = 6 kHz. The snubber capacitor has a value Cs = 58 nF.

Determine a suitable value for the snubber resistor Rs assuming a worst case minimum duty-cycle of 10%.

Please specify your answer in units of Ω to 2 decimal places.

## Given values
- DC supply voltage, Vdc = 200 V
- PWM frequency, fpwm = 6 kHz
- Snubber capacitor, Cs = 58 nF
- Worst-case minimum duty cycle, δmin = 10% = 0.10

## What the question is asking for
Find a suitable snubber resistor Rs, in ohms, to 2 decimal places.

## Correct answer
Rs = 43.54 Ω

## Method summary
The snubber capacitor Cs discharges through Rs when the MOSFET is on. The worst-case available discharge time is the minimum on-time:

ton,min = δmin / fpwm = 0.10 / 6000 = 16.67 μs

For the ELE336 design rule, the RC circuit is assumed settled after 3 rise/fall times. The 10%-90% rise/fall time is:

tr ≈ 2.2 Rs Cs

Therefore:

ton,min = 3 × 2.2 × Rs × Cs = 6.6 Rs Cs

Rearrange:

Rs = ton,min / (6.6 Cs)

Substitute:

Rs = 16.67 μs / (6.6 × 58 nF) = 43.54 Ω

Equivalent compact form for δmin = 0.10:

Rs = Tpwm / (66 Cs)

## Formula / equation source
- Circuit reasoning: Cs must discharge through Rs during MOSFET on-time.
- RC transient rule: a first-order RC circuit is treated as settled after approximately 3 rise/fall intervals.
- 10%-90% RC rise/fall-time approximation: tr ≈ 2.2 Rs Cs.
- PWM timing: ton,min = δmin / fpwm.

## Must-know concept
For a turn-off snubber, Rs is not chosen from Vdc directly in this step. Rs is chosen so that Cs is reset before the next turn-off event; the minimum duty cycle gives the shortest MOSFET on-time and is therefore the worst case for capacitor discharge.

## Date archived
2026-05-29

## Original image filename
image.png

## GitHub image storage
Image not stored in GitHub for this entry. User will keep the image in a separate Word document and use the caption above to associate the image with this archived question.

## Duplicate-check result
New question. No duplicate was found in the existing manifest, and repository search found no matching stored question/values before archiving.
