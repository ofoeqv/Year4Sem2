# Boost converter diode peak inverse voltage expression

## Caption for Word image document
Boost converter theory-expression question: when the transistor is on, the diode is reverse biased with its anode near 0 V and its cathode at the output voltage, so the diode peak inverse voltage is Vo; correct option B.

## Where this belongs / folder path
`ta questions/theory expressions/boost/diode-peak-inverse-voltage-normal-operation/description.md`

## Question title / short name
Boost diode peak inverse voltage

## Category
Theory expressions

## Subcategory
Boost converter / diode voltage stress

## Key topic
Identifying the peak inverse voltage across the boost converter diode during normal operation.

## Full visible question text
The circuit diagram below shows a Boost converter.

What is the peak inverse voltage (PIV) that the diode will experience during normal operation?

Options shown:
- A: `Vdc`
- B: `Vo`
- C: `Vo − Vdc`
- D: `Vo + Vdc`

## Given values
- Converter: Boost converter
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Device of interest: diode `D`
- Quantity: diode peak inverse voltage / reverse voltage stress

## What the question is asking for
The symbolic expression for the peak inverse voltage experienced by the boost diode.

## Correct answer
`B. Vo`

## Method summary
The diode experiences its maximum reverse voltage when the transistor is conducting.

During transistor on-time:

- The switch node / diode anode is pulled close to 0 V.
- The diode cathode remains connected to the output capacitor at approximately `Vo`.
- The diode is reverse biased.

Therefore the diode reverse voltage magnitude is:

`PIV = Vo − 0 = Vo`

So the diode peak inverse voltage is:

`PIV_D = Vo`

## Formula / equation source
- Circuit reasoning: during boost switch-on, the transistor clamps the diode anode to the lower rail while the output capacitor holds the diode cathode at `Vo`.
- Device voltage-stress reasoning: PIV is the maximum reverse voltage across the diode.

## Must-know concept
In a boost converter, the diode must block the output voltage when the switch is on. That is why the diode PIV is `Vo`, not `Vdc`.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded screenshot.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: new theory-expression question.

- Repository search found no exact existing archive entry for boost diode peak inverse voltage.
- Similar archive entry exists for boost maximum transistor voltage, but that asks for transistor voltage stress. This question asks for diode reverse voltage stress, so it is a distinct device-stress category.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
