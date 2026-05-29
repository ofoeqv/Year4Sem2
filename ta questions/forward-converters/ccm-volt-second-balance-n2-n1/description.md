# Forward converter CCM volt-second balance

## Caption for your Word image document
Forward converter CCM volt-second-balance question: during the switch-on interval the secondary applies approximately (N2/N1)Vdc to the output filter, so the inductor voltage is (N2/N1)Vdc − Vo; during the freewheel interval the inductor voltage is −Vo.

## Question title / short name
Forward converter volt-second balance equation for L

## Category
forward-converters

## Subcategory
ccm-volt-second-balance

## Key topic
Selecting the correct inductor volt-second balance equation for a forward converter in CCM.

## Full visible question text
The circuit diagram below shows a Forward converter.

The voltage and currents in the circuit can be separated into an average quantity and a ripple quantity such that x(t) = X̄ + Δx(t), where x(t) is the signal, X̄ is the average and Δx(t) is the ripple function.

If the circuit is operated in continuous current mode with a duty ratio δ and the transformer has a turn ratio N1:N2:N3, the volt-seconds balance equation for L is given by:

A. δ(N2/N1 × Vdc − Vo) − (1−δ)Vo = 0

B. δ(Vdc − Vo) − (1−δ)Vo = 0

C. δ(Vdc − N2/N1 × Vo) − (1−δ)Vo = 0

D. δ(N2/N1 × Vdc − Vo) + (1−δ)Vo = 0

## Given values
- Converter type: forward converter
- Operating mode: continuous current mode (CCM)
- Duty ratio: δ
- Transformer turns ratio: N1:N2:N3

## What the question is asking for
Choose the correct volt-second balance equation for the output inductor L.

## Correct answer
A. δ(N2/N1 × Vdc − Vo) − (1−δ)Vo = 0

## Method summary
During the switch-on interval, the primary voltage is transferred to the secondary according to the turns ratio:

vsec = (N2/N1)Vdc

The output inductor sees:

vL,on = (N2/N1)Vdc − Vo

During the switch-off/freewheel interval, the output inductor freewheels through D1, so the left side of L is approximately clamped to 0 V:

vL,off = −Vo

Volt-second balance in steady state requires the average inductor voltage over one switching period to be zero:

δvL,on + (1−δ)vL,off = 0

Therefore:

δ[(N2/N1)Vdc − Vo] + (1−δ)(−Vo) = 0

which is:

δ(N2/N1 × Vdc − Vo) − (1−δ)Vo = 0

## Formula / equation source
- Formula sheet: volt-second balance, integral of vL over one PWM period equals zero in steady state.
- Circuit reasoning: transformer secondary voltage is (N2/N1)Vdc during switch-on.
- Circuit reasoning: freewheel diode clamps the inductor input node during switch-off, giving vL = −Vo.

## Must-know concept
A forward converter behaves like an isolated buck converter: during switch-on, the inductor is driven by the transformed input voltage; during switch-off, the inductor freewheels and its voltage is negative.

## Date archived
2026-05-29

## Original image filename
image.png

## GitHub image storage
Image not stored in GitHub for this entry. User will keep the image in a separate Word document and use the caption above to associate the image with this archived question.

## Duplicate-check result
New question. No duplicate was found in the existing manifest, and repository search found no matching stored question/values before archiving.
