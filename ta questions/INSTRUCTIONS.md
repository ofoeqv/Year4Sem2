# ELE336 TA Question Archive Instructions

This file is the handoff seed for continuing the ELE336 Power Electronics TA/exam-question archive workflow.

## Repository setup

- Repository: `ofoeqv/Year4Sem2`
- Branch: `power-elec`
- Archive root: `ta questions`
- Manifest: `ta questions/manifest.json`
- Store Markdown descriptions only. Do not store the question images in GitHub.
- Images are kept separately in the user's Word document. Each archive entry must provide a caption for that Word document.

## Workflow for each question

1. Read the prompt and image carefully.
2. Classify the question by converter/topic category and subcategory.
3. Extract values, units, requested quantity, and answer format.
4. Check `ta questions/manifest.json`.
5. Search the repository using the converter type, requested element, key equation, visible values, and distinctive wording.
6. Decide whether the question is an exact duplicate, a duplicate-logic candidate, a distinct category question, or a new question.
7. If clearly new, create the Markdown archive file and update the manifest.
8. If ambiguous, present the arguments for and against archiving, then ask the user before saving.
9. If the user says skip, do not archive.

## Duplicate rules

Duplicates are not only about raw numbers. A question can be duplicate logic even when the numerical values are different.

### Exact duplicate

Treat as exact duplicate when the converter/circuit family, requested quantity, method, wording, and visible values are effectively the same as an existing archive entry.

Action: report the existing path and do not archive.

### Duplicate-logic candidate

Treat as duplicate logic when the question has the same converter/circuit family, same requested element, same equation/toolset, and same method structure, with only numerical values changed.

Examples:

- Turn-on snubber inductor sizing using `Ls = Vdc tr / IL` with different `Vdc` or `IL`.
- Buck-boost CCM inductor ripple using the same duty-ratio and `vL = L di/dt` method with different values.
- Closed-loop buck `Vdc` from `C2`, feedback divider, PWM duty, and `Vo = delta Vdc`, with only resistor values changed.

Action: tell the user it is a duplicate-logic candidate, give the answer if useful, and ask whether to archive it as a parameter variant or skip.

### Distinct category question

Do not treat a question as duplicate just because it uses the same broad principle. If it belongs to a different converter category, asks for a different balance equation, or is a reusable exam-question category, it may need its own archive entry.

Examples that should be considered separate categories:

- Buck converter CCM capacitor charge balance.
- Boost converter CCM capacitor charge balance.
- Boost converter CCM inductor volt-second balance.
- Buck-boost converter CCM inductor volt-second balance.
- Forward converter CCM volt-second balance.

These all use balance ideas, but the converter topology and circuit reasoning are different.

## Ambiguous-case rule

When a question looks similar but may be a distinct category, do not decide silently. Present:

1. Reasons to treat it as duplicate logic.
2. Reasons to treat it as a distinct category.
3. Your recommendation.
4. A question asking the user whether to archive or skip.

Example wording:

`This uses the same broad charge-balance idea, but it is a different converter topology and a useful separate revision category. I recommend archiving it under buck converters. Do you want me to save it or skip it?`

## Folder conventions

Use the existing folders unless the user asks for a new one:

- `ta questions/buck-converters/`
- `ta questions/Boost convertes/`
- `ta questions/buck-boost-converter/`
- `ta questions/forward-converters/`
- `ta questions/h-bridge/`
- `ta questions/snubbers/`
- `ta questions/semiconductor-losses/`
- `ta questions/mosfet-heat-questions/`
- `ta questions/feedback style/`
- `ta questions/graph questions/`

Keep using `Boost convertes` as the existing folder name unless the user asks to rename it.

## Required Markdown sections

Each archived question file must include:

- Caption for Word image document.
- Folder path.
- Question title / short name.
- Category.
- Subcategory.
- Key topic.
- Full visible question text.
- Given values.
- What the question is asking for.
- Correct answer if solvable.
- Method summary.
- Formula / equation source.
- Must-know concept.
- Date archived.
- Original image filename if available.
- GitHub image storage note.
- Duplicate-check result.
- Uncertainty.

## Manifest rules

After creating a new archive file, update `ta questions/manifest.json` with at least:

- `id`
- `question_title`
- `category`
- `subcategory`
- `key_topic`
- `path`
- `description_file`
- `asked_for`
- `correct_answer`
- `date_archived`

## Response style to the user

When replying after archiving:

- State duplicate status first.
- Give the archive path.
- Give the correct answer.
- Show a concise calculation.
- Provide the Word caption.

When solving or tutoring:

- Start with category/subcategory.
- Say whether equations come from the formula sheet or circuit reasoning.
- Briefly derive non-formula-sheet equations.
- Include a short must-know concept.
- Check image values before calculating.

## Critical reminder

If there are arguments both for and against treating a question as duplicate logic, present both sides and ask the user before acting. A new converter topology or a new balance-equation category can justify archiving even when the broad method is similar.
