# Turn-off snubber capacitor for MOSFET drain-source voltage rise time

## Caption for Word image document
Turn-off snubber capacitor-sizing question: a MOSFET switch with Vdc = 138 V and inductive load current IL = 10 A uses a turn-off snubber capacitor Cs to set the drain-source voltage rise time to 1 µs; using iC = C dv/dt gives Cs = 72.46 nF.

## Where this belongs / folder path
`ta questions/snubbers/turn-off-snubber-capacitor-vdc138-il10-trise1us/description.md`

## Question title / short name
Turn-off snubber capacitor from VDS rise time

## Category
Snubbers

## Subcategory
Turn-off snubber / capacitor sizing

## Key topic
Sizing the turn-off snubber capacitor so the MOSFET drain-source voltage rises over a specified time while the inductive load current is handed to the snubber.

## Full visible question text
Question 1. The circuit below shows a MOSFET switch with a turn-off snubber operating from a DC supply voltage Vdc = 138 V. Assume the handover of the inductive load current IL = 10 A from the MOSFET to the snubber occurs instantaneously.

Calculate a value for Cs to provide a vDS rise time tr = 1 µs.

Please specify your answer in units of nF to 2 decimal places.

## Given values
- DC supply voltage: `Vdc = 138 V`
- Inductive load current: `IL = 10 A`
- Required drain-source voltage rise time: `tr = 1 µs`
- Snubber capacitor: `Cs`
- Snubber resistor: `Rs`
- Snubber diode: `Ds`
- Assumption: load current handover from MOSFET to snubber is instantaneous

## What the question is asking for
The required turn-off snubber capacitance `Cs`, in nanofarads.

## Correct answer
`Cs = 72.46 nF`

## Method summary
During MOSFET turn-off, the snubber capacitor takes the load current and controls the rise rate of the MOSFET drain-source voltage. With instantaneous current handover, the capacitor current is approximately:

`iCs = IL`

Using the capacitor equation:

`iC = C dv/dt`

Rearrange for capacitance:

`Cs = IL tr / Vdc`

Substitute:

`Cs = 10 × 1e−6 / 138`

`Cs = 72.46e−9 F = 72.46 nF`

## Formula / equation source
- Formula sheet: `iC = C dvC/dt`.
- Circuit reasoning: during the turn-off transition, the snubber capacitor current is approximately the load current and the capacitor voltage rises from 0 V to `Vdc` over `tr`.
- Derived sizing equation: `Cs = IL tr / Vdc`.

## Must-know concept
A turn-off snubber capacitor slows the rise of MOSFET drain-source voltage. Bigger `Cs` means the same load current charges the capacitor more slowly, so `vDS` rises more slowly.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded circuit screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new snubber category question.

- Manifest check: existing snubber entries include turn-off snubber resistor sizing and turn-on snubber inductor sizing, but no turn-off snubber capacitor sizing entry.
- Repository search: no exact match found for turn-off snubber capacitor `Cs`, `Vdc = 138 V`, `IL = 10 A`, and `tr = 1 µs`.
- Decision: archived under snubbers as a distinct turn-off capacitor-sizing question.

## Uncertainty
No visible value uncertainty. The prompt clearly gives `Vdc = 138 V`, `IL = 10 A`, and `tr = 1 µs`.
