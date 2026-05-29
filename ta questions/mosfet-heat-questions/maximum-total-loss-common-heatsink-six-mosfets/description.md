# Maximum allowed total losses for MOSFETs on common heatsink

## Caption for Word image document
MOSFET heatsink thermal-limit question: six MOSFET devices share a common heatsink with thermal resistance 1 °C/W; to keep the device case temperature below 98 °C at the worst-case ambient temperature of 43 °C, the maximum total device loss is 55.00 W.

## Where this belongs / folder path
`ta questions/mosfet-heat-questions/maximum-total-loss-common-heatsink-six-mosfets/description.md`

## Question title / short name
Maximum total losses for six MOSFETs on a common heatsink

## Category
MOSFET heat questions

## Subcategory
Thermal resistance / common heatsink power-loss limit

## Key topic
Using heatsink thermal resistance and worst-case ambient temperature to calculate maximum allowed total power dissipation.

## Full visible question text
A power converter employing six MOSFET devices is mounted onto a common heatsink with a thermal resistance of 1 ˚ºC / W.

If the device case temperature is to be kept below 98 ºC, in an environment with an ambient temperature changing in the range from 1 ºC to 43 ºC, what are the maximum allowed total losses (in watts) of all the devices?

Please specify your answer in units of W to 2 decimal places.

## Given values
- Number of MOSFET devices: `6`
- Common heatsink thermal resistance: `Rθ = 1 °C/W`
- Maximum allowed device case temperature: `Tcase,max = 98 °C`
- Ambient temperature range: `Tamb = 1 °C to 43 °C`
- Worst-case ambient temperature: `Tamb,max = 43 °C`

## What the question is asking for
The maximum allowed total losses of all six MOSFET devices combined, in watts.

## Correct answer
`Ptotal,max = 55.00 W`

## Method summary
Use the worst-case ambient temperature because it gives the smallest allowed temperature rise:

`ΔTmax = Tcase,max − Tamb,max`

`ΔTmax = 98 − 43 = 55 °C`

Thermal resistance relates temperature rise and total heat dissipated:

`Rθ = ΔT / P`

so:

`Ptotal,max = ΔTmax / Rθ = 55 / 1 = 55.00 W`

The six MOSFETs are mounted on the same heatsink, so the calculated value is the total allowed loss for all devices together, not per MOSFET.

## Formula / equation source
- Thermal circuit reasoning: `ΔT = P × Rθ`.
- Rearranged thermal-loss limit: `Pmax = (Tcase,max − Tamb,max)/Rθ`.

## Must-know concept
For heatsink questions, always use the worst-case ambient temperature. When several devices share one heatsink, the heatsink sees the total loss from all devices.

## Date archived
2026-05-29

## Original image filename
No image provided; text-only question.

## GitHub image storage note
No image stored in GitHub. User keeps any related images separately in a Word document and uses the caption above to link the Word image or text question to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic.

- Manifest check: no existing thermal-resistance/heatsink total-loss question found.
- Duplicate-logic check: not flagged as duplicate logic because existing archived questions concern converter ripple, snubbers, H-bridge average voltage, forward/buck-boost volt-second balance, and closed-loop buck feedback calculations, not heatsink thermal limits.
- Repository search: no exact repository match found for MOSFET heatsink, thermal resistance `1 °C/W`, case temperature `98 °C`, ambient range `1 °C to 43 °C`, or total allowed losses.

## Uncertainty
No value uncertainty. The question is text-only and clearly gives `Rθ = 1 °C/W`, `Tcase,max = 98 °C`, and ambient range `1 °C to 43 °C`.
