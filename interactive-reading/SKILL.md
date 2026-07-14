---
name: interactive-reading
description: Transform books, chapters, papers, courses, transcripts, meeting notes, or other static learning materials into an interactive mastery workflow. Use when the user wants to read efficiently, grasp a book's core content, build a learning map, extract arguments and concepts, diagnose blind spots, run Socratic study loops, create review questions or flashcards, produce project-facing reading notes, or apply a CC-style interactive learning method.
---

# Interactive Reading

## Core Idea

Turn "reading in author order" into "mastery in question order." Do not merely summarize. Build a path that starts from the learner's goal, extracts the book's core structure, diagnoses gaps, drills the important units, and ends with compression, transfer, and review.

Use this skill for books, articles, courses, podcasts, papers, meeting notes, and any static material that can become a study path.

## Workflow

1. Define the reading target.
   - Ask up to 4 diagnostic questions when the goal, background, or use case is unclear.
   - If the user already provides enough context, infer the profile and proceed.
   - Clarify whether the goal is: understand, decide, write, teach, build, create, invest, examine, or act.

2. Create or update the learning archive.
   - Capture: title, source type, source coverage, learner goal, prior knowledge, constraints, desired output, and success criteria.
   - Keep the archive concise and update it as new answers appear.

3. Extract the core content before teaching.
   - Identify the central question, author thesis, key concepts, argument chain, evidence/examples, methods, useful distinctions, blind spots, and skippable material.
   - Separate what the source says from interpretation, external knowledge, and user-specific transfer.

4. Build the numbered skeleton and learning map.
   - Decompose the material into major sections, then small learning units.
   - Give every claim, concept, method, example, and exercise a stable number.
   - Preserve author order only when it helps. Reorder by the learner's goal when useful.
   - Identify the minimum path, optional branches, dependencies, practice points, and outputs.
   - Mark each unit as: `must`, `useful`, `optional`, or `skip`.

5. Run interactive study loops.
   - For each selected unit, produce: core idea, why it matters, prerequisites, active recall, Socratic questions, transfer task, and mastery checkpoint.
   - If the learner answers incorrectly, do not give the final answer immediately. Reframe, lower the difficulty, or ask from another angle.
   - A unit is not mastered until the learner can restate it, give an example or counterexample, and apply it to their own context.

6. Compress the book into reusable forms.
   - Produce the smallest useful set: one-sentence thesis, one-page brief, 10 core ideas, concept table, argument chain, action/project implications, and review questions.

7. Produce artifacts and close the loop.
   - Prefer concrete outputs over summaries: study map, flashcards, chapter briefs, practice tasks, decision trees, essays, diagrams, implementation plans, teaching scripts, project notes, or final reading notes.
   - When the user asks for files, create Markdown files with stable numbered headings.
   - End substantial reading runs with a review pack: recall questions, flashcards, weak points, next reading/action, and whether the note is ready for knowledge-base export.
   - When the user asks to save a finished reading note into a knowledge base, hand off to the user's separate knowledge-base intake workflow instead of handling filing rules inside this skill.

## Operating Rules

- Avoid generic book summaries unless the user explicitly asks for one.
- Keep all claims grounded in the supplied material. If external knowledge is needed, say so and separate it from source-derived interpretation.
- Use Chinese by default when the user writes in Chinese.
- Keep each study unit small enough to teach, quiz, and apply in one sitting.
- Use stable numbering so later discussion can refer to "2.3" or "U14" without ambiguity.
- Make the learner do cognitive work: prediction, recall, comparison, application, critique, and teaching back.
- Prefer fewer high-value units over exhaustive coverage when the user wants efficient reading.
- Do not treat "finished reading" as "mastered." Check recall, explanation, counterexample, and transfer.
- Adapt questions by material type: cognitive books need bias/failure cases, business books need decision rules, creative books need project application, technical books need executable steps, and reflective books need personal meaning and behavior change.
- When material is missing, create a reusable reading protocol instead of pretending to know the text.
- Keep knowledge-base registration outside this skill. `interactive-reading` may produce the final note, but vault filing, reading logs, and long-term distillation status belong to the user's separate knowledge-base intake workflow.

## Output Modes

Choose the smallest useful mode:

- `diagnose`: Ask diagnostic questions and produce a learner profile.
- `intake`: Identify source type, source coverage, missing material, and reading strategy.
- `core`: Extract the central question, thesis, concepts, argument chain, examples, and skippable material.
- `skeleton`: Build a numbered book/course skeleton.
- `map`: Build a learning path with dependencies and priorities.
- `unit`: Turn one section into an interactive study unit.
- `socratic`: Generate progressive questions for a concept or claim.
- `mastery`: Test recall, explanation, counterexample, and transfer for one or more units.
- `compress`: Produce one-sentence, one-page, 10-idea, concept-table, and argument-chain summaries.
- `project`: Apply the book to a concrete project, decision, writing task, creative work, or behavior change.
- `review`: Create flashcards, recall questions, weak points, and a spaced review plan.
- `final-note`: Produce a finished reading note while preserving the user's own language and keeping knowledge-base export separate.
- `archive`: Maintain a compact learning archive across turns.
- `batch`: Produce multiple study units or files.

For detailed templates, read `references/templates.md` when generating structured outputs, file artifacts, mastery checks, compression summaries, project-facing notes, or review packs.
