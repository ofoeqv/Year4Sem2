# Flyback converter maximum transistor voltage expression

## Caption for Word image document
Flyback converter theory-expression question: when the transistor is off, the output voltage is reflected to the primary side and adds to the DC input, so the maximum transistor voltage is Vdc + (N1/N2)Vo; correct option A.

## Where this belongs / folder path
`ta questions/theory expressions/flyback/maximum-transistor-voltage/description.md`

## Question title / short name
Flyback maximum transistor voltage

## Category
Theory expressions

## Subcategory
Flyback converter / transistor voltage stress

## Key topic
Identifying the maximum transistor voltage in a flyback converter using reflected secondary voltage.

## Full visible question text
Consider the Flyback converter circuit shown below.

The flyback transformer has a turn ratio `N1:N2`. Which one of the expressions below correctly defines the maximum voltage experienced by the transistor?

Options shown:
- A: `Vdc + (N1/N2)Vo`
- B: `Vdc − (N1/N2)Vo`
- C: `Vdc`
- D: `(N1/N2)Vo`

## Given values
- Converter: Flyback converter
- Primary turns: `N1`
- Secondary turns: `N2`
- Input voltage: `Vdc`
- Output voltage: `Vo`
- Device of interest: transistor/switch

## What the question is asking for
The symbolic expression for the maximum transistor voltage.

## Correct answer
`A. Vdc + (N1/N2)Vo`

## Method summary
When the transistor is off, the secondary diode conducts and the output voltage is reflected back to the primary winding. The reflected output voltage on the primary side is:

`Vreflected = (N1/N2)Vo`

This reflected voltage adds to the input supply voltage across the transistor. Therefore the maximum ideal transistor voltage is:

`vS,max = Vdc + (N1/N2)Vo`

## Formula / equation source
- Transformer/coupled-inductor reasoning: secondary voltage reflects to the primary in proportion to the turns ratio `N1/N2`.
- Circuit reasoning: during flyback switch-off, the reflected output voltage adds to `Vdc` across the transistor.

## Must-know concept
Flyback switch voltage stress is higher than the input voltage because the transistor must block both the DC input and the output voltage reflected back through the transformer.

## Date archived
2026-05-30

## Original image filename
`image.png` from user-uploaded screenshot. The same question appeared twice in the uploaded group and is stored once only.

## GitHub image storage note
Image not stored in GitHub. User keeps the image separately in a Word document and uses the caption above to link the Word image to this archived GitHub question.

## Duplicate-check result
Status: stored once. The uploaded set contained the same flyback maximum-transistor-voltage question twice, so only one archive file was created.

## Uncertainty
No numerical uncertainty. This is a symbolic multiple-choice theory question.
