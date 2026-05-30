# Buck converter DCM diode conduction time from inductor-current waveform

## Caption for Word image document
Graph-based buck converter DCM diode-conduction-time question: the inductor current rises during switch on-time with slope (Vdc − Vo)/L and falls during diode conduction with slope −Vo/L, so tdiode = ((Vdc − Vo)/Vo) ton; correct option A.

## Where this belongs / folder path
`ta questions/graph questions/buck-dcm-diode-conduction-time-expression.md`

## Question title / short name
Buck DCM diode conduction time expression

## Category
Graph questions

## Subcategory
Buck converter / DCM diode conduction interval

## Key topic
Using the triangular DCM inductor-current waveform to derive the diode conduction time in a buck converter.

## Full visible question text
The waveform below shows the inductor current for a Buck converter operating in discontinuous current mode (DCM).

Which of the following expressions correctly defines the diode conduction time `tdiode`?

Options shown:
- A: `tdiode = ((Vdc − Vo)/Vo) ton`
- B: `tdiode = ((Vdc − Vo)/Vdc) ton`
- C: `tdiode = (Vdc/(Vdc − Vo)) ton`
- D: `tdiode = (Vo/(Vdc − Vo)) ton`

## Given values
- Converter: Buck converter
- Operating mode: DCM
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Switch on-time: `ton`
- Diode conduction time: `tdiode`
- Inductor current starts at zero in each switching period

## What the question is asking for
The symbolic expression for the diode conduction time `tdiode` in buck converter DCM.

## Correct answer
`A. tdiode = ((Vdc − Vo)/Vo) ton`

## Method summary
During switch on-time, the inductor voltage is:

`vL,on = Vdc − Vo`

So the inductor current rises with slope:

`diL/dt = (Vdc − Vo)/L`

The peak current at the end of `ton` is:

`Ipk = ((Vdc − Vo)/L) ton`

During diode conduction, the switch is off and the inductor voltage is approximately:

`vL,off = −Vo`

So the inductor current falls with magnitude of slope:

`Vo/L`

The time required for the current to fall from `Ipk` to zero is:

`tdiode = Ipk / (Vo/L)`

Substitute `Ipk`:

`tdiode = [((Vdc − Vo)/L) ton] / (Vo/L)`

Therefore:

`tdiode = ((Vdc − Vo)/Vo) ton`

## Formula / equation source
- Formula sheet: `vL = L diL/dt`.
- Circuit reasoning: buck ON interval has `vL = Vdc − Vo`.
- Circuit reasoning: buck diode-conduction interval has `vL = −Vo`.
- Waveform reasoning: DCM current ramps up from zero, then ramps back down to zero during diode conduction.

## Must-know concept
In buck DCM, the diode conduction time is set by how quickly the inductor current decays to zero. The decay slope is controlled by `Vo`, not by `Vdc`.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded waveform/options screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new graph question.

- Repository search found no exact existing archive entry for a buck DCM diode conduction time waveform expression.
- Existing graph entries include boost DCM maximum transistor current and buck CCM capacitor-ripple expression, but this asks for buck DCM diode conduction interval, so it is a distinct graph-question type.

## Uncertainty
No visible value uncertainty. This is a symbolic multiple-choice graph question rather than a numerical calculation.
