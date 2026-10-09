# Reading Study Guide Skill

Create a bilingual, evidence-grounded study guide for a weekly set of course readings. The skill focuses on deep questions tied to the user's weekly theme and produces one formatted Word document.

## What it does

- Reads the supplied course PDFs and maps each reading's argument, evidence, assumptions, scope, and limitations.
- Reflects the user-provided weekly theme in Chinese and English.
- Produces a Chinese-first, bilingual overview, a one-sentence takeaway, and exactly 10 deep comprehension questions per reading, with substantial bilingual answer points and verifiable source page references.
- Combines the guides into one DOCX named `Week X Reading Note.docx`.
- Formats Chinese text in SimSun, English text in Times New Roman, and body text at 12 pt with single spacing.

## Use with Codex

Install the `reading-study-guide` folder as a Codex skill, then restart or refresh Codex's skill list if needed. Example installation command:

```sh
python3 "$HOME/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo OWNER/REPOSITORY --path skills/reading-study-guide
```

Replace `OWNER/REPOSITORY` with the public repository location. The skill is configured for explicit invocation, so it will not automatically process unrelated PDFs.

Example prompt:

```text
Use $reading-study-guide for this week's assigned readings.
Weekly theme: [provide the course theme]
Week: [provide the week number]
Create one DOCX study guide from the attached PDFs.
```

The weekly theme and source PDFs are required. If the week number is unknown, the skill asks or uses `X` rather than guessing.

## Requirements and limits

- Provide source PDFs that the user has permission to process. The skill does not fetch or replace missing readings.
- Page references are included only when verifiable. Scanned or unreadable material may need OCR or visual inspection; uncertain references are omitted and limitations are reported outside the DOCX.
- The skill's analysis is grounded in supplied sources. It does not claim that automated checks prove every interpretation correct.
- A DOCX-capable document workflow is required to create and verify the final Word file.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE).
