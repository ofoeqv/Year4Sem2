# H-bridge average load voltage

## Caption for your Word image document
H-bridge converter average-load-voltage question: four MOSFETs and four antiparallel diodes form a full bridge connected to a 400 V DC link, with a resistive load of 127 Ω and switch S1 operated at 35% duty cycle.

## Question title / short name
H-bridge average voltage from S1 duty cycle

## Category
h-bridge

## Subcategory
average-load-voltage / resistive-load

## Key topic
Average output voltage of a bipolar H-bridge switching waveform.

## Full visible question text
A H-bridge converter employing four MOSFET devices and four diodes is connected to a dc source of 400 V and operates at 8 kHz. The duty cycle of switch S1 is 35 %. The circuit diagram is included below.

Calculate the average voltage across a resistive load of R = 127 Ω.

Please specify your answer in units of V to 2 decimal places.

## Given values
- DC-link voltage, Vdc = 400 V
- PWM frequency, fpwm = 8 kHz
- Duty cycle of S1, d = 35% = 0.35
- Load resistance, R = 127 Ω
- Load type: resistive

## What the question is asking for
Calculate the average voltage across the resistive load.

## Correct answer
Vload,avg = -120.00 V

## Method summary
For a bipolar full H-bridge, when S1 and the opposite diagonal switch conduct, the load voltage is +Vdc. During the complementary interval, the opposite diagonal pair gives -Vdc.

The average load voltage is:

Vload,avg = Vdc(2d - 1)

Substitute:

Vload,avg = 400(2 × 0.35 - 1) = 400(−0.30) = −120 V

So:

Vload,avg = −120.00 V

## Formula / equation source
- Circuit reasoning: H-bridge diagonal switching gives +Vdc for duty d and −Vdc for duty 1−d.
- Average waveform calculation: Vavg = dVdc + (1−d)(−Vdc) = Vdc(2d−1).
- Related inverter lecture relation: full-bridge average output voltage is vL = Vdc(2d−1).

## Must-know concept
For a bipolar H-bridge, 50% duty gives zero average load voltage. A duty below 50% gives a negative average voltage, and a duty above 50% gives a positive average voltage, depending on the chosen load-voltage reference direction.

## Date archived
2026-05-29

## Original image filename
image.png

## GitHub image storage
Image not stored in GitHub for this entry. User will keep the image in a separate Word document and use the caption above to associate the image with this archived question.

## Duplicate-check result
New question. No duplicate was found in the existing manifest, and repository search found no matching stored question/values before archiving.
