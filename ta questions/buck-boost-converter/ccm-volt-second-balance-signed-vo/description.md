# Buck-boost converter CCM volt-second balance

## Caption for your Word image document
Buck-boost converter CCM volt-second-balance question: during switch-on the inductor voltage is +Vdc, and during diode-conduction/switch-off the inductor voltage is Vo, where Vo is drawn with negative polarity for the inverting buck-boost output.

## Question title / short name
Buck-boost converter volt-second balance equation for L

## Category
buck-boost-converter

## Subcategory
ccm-volt-second-balance

## Key topic
Selecting the correct inductor volt-second balance equation for a buck-boost converter in CCM.

## Full visible question text
The circuit diagram below shows a Buck-boost converter.

The voltage and currents in the circuit can be separated into an average quantity and a ripple quantity such that x(t) = X̄ + Δx(t), where x(t) is the signal, X̄ is the average and Δx(t) is the ripple function.

If the circuit is operated in continuous current mode with a duty ratio δ, the volt-seconds balance equation for L is given by:

A. δVdc + (1−δ)Vo = 0

B. δVdc − (1−δ)(Vdc − Vo) = 0

C. δ(Vdc − Vo) + (1−δ)(Vdc − Vo) = 0

D. (1−δ)Vdc + (1−δ)(Vdc − Vo) = 0

## Given values
- Converter type: buck-boost converter
- Operating mode: continuous current mode (CCM)
- Duty ratio: δ

## What the question is asking for
Choose the correct volt-second balance equation for the inductor L.

## Correct answer
A. δVdc + (1−δ)Vo = 0

## Method summary
For the inverting buck-boost converter, during switch-on:

vL,on = Vdc

During switch-off, the diode conducts and the inductor transfers energy to the output. With the output voltage drawn using the converter’s negative output polarity, the inductor voltage in this interval is:

vL,off = Vo

Steady-state volt-second balance requires:

δvL,on + (1−δ)vL,off = 0

Therefore:

δVdc + (1−δ)Vo = 0

This also leads to the standard inverting buck-boost conversion relation:

Vo = −Vdc δ/(1−δ)

## Formula / equation source
- Formula sheet: volt-second balance, integral of vL over one PWM period equals zero in steady state.
- Circuit reasoning: vL = Vdc during switch-on.
- Circuit reasoning: vL = Vo during switch-off using the signed output-voltage convention shown in the diagram.

## Must-know concept
For an inverting buck-boost converter, Vo is negative relative to the input return. That is why the off-time inductor voltage can be written as Vo, and the volt-second balance becomes δVdc + (1−δ)Vo = 0.

## Date archived
2026-05-29

## Original image filename
image.png

## GitHub image storage
Image not stored in GitHub for this entry. User will keep the image in a separate Word document and use the caption above to associate the image with this archived question.

## Duplicate-check result
New question. No duplicate was found in the existing manifest, and repository search found no matching stored question/values before archiving.
