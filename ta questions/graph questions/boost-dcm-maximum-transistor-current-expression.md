# Boost converter DCM maximum transistor current from waveform

## Caption for Word image document
Graph-based boost converter DCM transistor-current question: during switch on-time, the boost inductor has Vdc across it, so the transistor current rises linearly to iS(max) = (Vdc/L) ton; correct option B.

## Where this belongs / folder path
`ta questions/graph questions/boost-dcm-maximum-transistor-current-expression.md`

## Question title / short name
Boost DCM maximum transistor current expression from waveform

## Category
Graph questions

## Subcategory
Boost converter / DCM inductor-current waveform

## Key topic
Finding the maximum transistor current in a boost converter operating in discontinuous current mode using the inductor-current ramp during switch on-time.

## Full visible question text
The figure below shows the inductor current waveform for a boost converter operating in discontinuous current mode.

If the circuit is operated from a DC input Vdc, with a switch on-time ton and produces an output voltage Vo, which one of the following expressions correctly defines the maximum current experienced by the transistor?

Options shown:
- A: `iS(max) = ((Vdc − Vo)/L) ton`
- B: `iS(max) = (Vdc/L) ton`
- C: `iS(max) = (Vo/L) ton`
- D: `iS(max) = ((Vdc + Vo)/L) ton`

## Given values
- Converter: Boost converter
- Operating mode: DCM
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Switch on-time: `ton`
- Inductor: `L`

## What the question is asking for
The symbolic expression for the maximum current experienced by the transistor.

## Correct answer
`B. iS(max) = (Vdc/L) ton`

## Method summary
In a boost converter, during Mode 1 the transistor is on and the diode is off. The input voltage is applied directly across the inductor:

`vL = Vdc`

Using the inductor relation:

`vL = L diL/dt`

so:

`diL/dt = Vdc/L`

In DCM, the inductor current begins at zero at the start of the on-time and rises linearly during `ton`, so the peak inductor current is:

`ΔIL = (Vdc/L) ton`

During the on-time, the transistor carries the inductor current, so:

`iS(max) = (Vdc/L) ton`

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: boost converter Mode 1 has the switch on, diode off, and `vL = Vdc`.
- Waveform reasoning: DCM current starts from zero and ramps to its peak during `ton`.

## Must-know concept
For boost converter switch-on mode, the inductor is being charged directly from the input supply. That is why the slope is `Vdc/L`, not `(Vdc − Vo)/L`.

## Date archived
2026-05-29

## Original image filename
`image.png` from user-uploaded graph/options screenshots.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new, not duplicate logic within the archive.

- Manifest check: no existing archived graph question for boost DCM maximum transistor current expression.
- Duplicate-logic check: no archived question currently asks for maximum transistor/switch current from a boost DCM waveform.
- Repository search: no exact repository match found for boost DCM maximum transistor current, `iS(max) = (Vdc/L) ton`, or the graph-based multiple-choice wording.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice graph question rather than a numerical calculation.
