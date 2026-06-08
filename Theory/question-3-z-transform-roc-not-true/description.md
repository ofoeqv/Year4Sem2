# Question 3 - Z-transform Region of Convergence (ROC)

## Category
Theory

## Topic
Z-transform and Region of Convergence (ROC)

## Question
Which of the following is **NOT** true of the Z-transform's Region of Convergence (ROC)?

## Options
A. A finite length sequence always has a ROC that covers the whole Z plane, apart from the origin.

B. An anti-causal sequence has a ROC that is a disc.

C. A causal sequence has a ROC that is donut-shaped.

D. A Z-transform is only fully defined if the ROC is also stated.

## Correct Answer
**C. A causal sequence has a ROC that is donut-shaped.**

## Explanation
For a causal/right-sided sequence, the ROC extends outward from the outermost pole:

\[
|z| > r
\]

So it is the outside of a circle, not a donut-shaped annulus.

A donut-shaped ROC is associated with a two-sided sequence, where the ROC lies between two poles:

\[
r_1 < |z| < r_2
\]

An anti-causal/left-sided sequence usually has an ROC that extends inward, so it is a disc-type region:

\[
|z| < r
\]

## Must-know concept
Causal/right-sided sequence: ROC is outside the outermost pole.  
Anti-causal/left-sided sequence: ROC is inside the innermost pole.  
Two-sided sequence: ROC is a ring/donut between poles.

## Duplicate check
Searched the repository for:

- `Z-transform Region of Convergence ROC causal sequence donut shaped anti-causal finite length sequence`
- `Question 3 Z-transform ROC Region of Convergence`

No duplicate was found before archiving.

## Source
Original uploaded image filename: `image.png`

## Date archived
2026-06-08
