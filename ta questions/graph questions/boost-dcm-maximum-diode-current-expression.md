# Boost converter DCM maximum diode current from waveform

## Caption for Word image document
Graph-based boost converter DCM diode-current question: the diode current reaches its maximum at the start of the diode-conduction interval, equal to the peak inductor current built during switch on-time, so iD(max) = (Vdc/L) ton; correct option B.

## Where this belongs / folder path
`ta questions/graph questions/boost-dcm-maximum-diode-current-expression.md`

## Question title / short name
Boost DCM maximum diode current expression from waveform

## Category
Graph questions

## Subcategory
Boost converter / DCM inductor-current waveform / diode current peak

## Key topic
Finding the maximum diode current in a boost converter operating in discontinuous current mode using the inductor-current ramp and the start of diode conduction.

## Full visible question text
The figure below shows the inductor current waveform for a boost converter operating in discontinuous current mode.

If the circuit is operated from a DC input `Vdc`, with a switch on-time `ton` and produces an output voltage `Vo`, which one of the following expressions correctly defines the maximum current experienced by the diode?

Options shown:
- A: `iD(max) = ((Vdc − Vo)/L) ton`
- B: `iD(max) = (Vdc/L) ton`
- C: `iD(max) = (Vo/L) ton`
- D: `iD(max) = ((Vdc + Vo)/L) ton`

## Given values
- Converter: Boost converter
- Operating mode: DCM
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Switch on-time: `ton`
- Inductor: `L`

## What the question is asking for
The symbolic expression for the maximum current experienced by the diode.

## Correct answer
`B. iD(max) = (Vdc/L) ton`

## Method summary
During Mode 1, the transistor is on and the diode is off. The input voltage is applied directly across the inductor:

`vL = Vdc`

Using the inductor relation:

`vL = L diL/dt`

so:

`diL/dt = Vdc/L`

In DCM, the inductor current starts at zero and rises linearly during `ton`, so the peak inductor current is:

`ΔIL = (Vdc/L) ton`

When the transistor turns off, the diode conducts. At the start of diode conduction, the diode current equals the peak inductor current, so:

`iD(max) = ΔIL = (Vdc/L) ton`

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: boost converter Mode 1 has switch on, diode off, and `vL = Vdc`.
- Waveform reasoning: in DCM the inductor current starts from zero and ramps to its peak during `ton`; the diode current is maximum at the beginning of the diode-conduction interval.

## Must-know concept
In a DCM boost converter, the diode does not conduct during switch on-time. However, its maximum current is still set by the peak inductor current that was built up during on-time.

## Date archived
2026-05-31

## Original image filename
`image.png` from user-uploaded graph/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: archived as a distinct requested-device question.

- Manifest check: an existing related entry asks for maximum transistor current in a boost DCM waveform, but not maximum diode current.
- Duplicate-logic check: the equation value is the same as the transistor-current peak because both are tied to the peak inductor current, but the requested element is different: diode current rather than transistor current.
- Repository search: no exact repository match found for boost DCM maximum diode current, `iD(max) = (Vdc/L) ton`, or the graph-based diode-current multiple-choice wording.
- Decision: archived because the user’s rules treat a different requested element/device current as a distinct useful revision category.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice graph question rather than a numerical calculation.
