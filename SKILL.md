---
name: reading-study-guide
description: Create a bilingual, source-grounded weekly reading study guide from course PDFs. Use when explicitly invoked to analyze assigned readings, connect them to a supplied weekly theme, develop deep comprehension questions, and deliver one formatted Word document.
---

# Reading Study Guide

Create one rigorous, bilingual Word study guide for a weekly set of assigned readings. This skill is for academic or course reading assignments when explicitly invoked. Do not apply it automatically to unrelated PDFs or general document tasks.

## Inputs and scope

- Use the user's supplied PDF files as the primary sources. Read every supplied source before drafting.
- The user should provide the weekly course theme. If it is missing, ask for it before drafting questions. Reflect the supplied theme back in concise Chinese and English bullet points in the conversation and include those theme points near the start of the Word document.
- If the week number is known from the user or course materials, use it in the output filename. If it is not known, ask or use the literal `X`; do not guess.
- If a source PDF is missing or inaccessible, explain what is needed and ask the user to upload it or provide its path. Do not claim completion without a successfully created DOCX.
- Prepare one guide per reading, then combine the guides into a single final DOCX for that weekly batch unless the user requests a comparison or another structure.

## Read and map the argument

Read the full source when possible and build an evidence-based understanding map before writing:

- central problem or research question and thesis;
- argument steps, causal or conceptual mechanisms, and links among claims;
- evidence, examples, data, methods, or reasoning and what they can establish;
- key concepts, assumptions, scope conditions, and definitions;
- limitations, caveats, counterarguments, and open questions;
- implications and how the reading supports, complicates, or challenges the supplied weekly theme.

Stay grounded in the supplied sources. Do not import outside facts unless the user asks. Keep the author's explicit claims separate from your interpretation, and label inference as inference.

## Study guide contents

Write in Chinese and English, with Chinese first and the corresponding English immediately after it. For each reading include:

1. **文章内容概括 / Article overview:** Explain the question, argument, approach, and main findings in accessible, structured detail.
2. **一句话核心结论 / One-sentence takeaway:** One concise sentence in each language.
3. **十道理解题 / Ten comprehension questions:** Exactly 10 substantive questions, each in Chinese and English, with answer analysis in both languages. Format every answer point as a bullet.
4. **原文页码 / Page references:** Cite PDF page numbers beside relevant claims and answer points when verifiable. If printed pagination differs, identify both. Never invent page references.

### Question design and answer depth

Design questions to test understanding of the article's core argument and its relationship to the weekly theme, not simple recall. Prefer high-leverage “why,” “how,” and “under what conditions” questions. Across the 10 questions, cover as relevant:

- the central problem and thesis;
- the reasoning or mechanism connecting premises to conclusions;
- how evidence supports the claims and what it does not establish;
- assumptions, scope, and conditions under which the argument holds;
- limitations, plausible alternatives, or tensions;
- consequences or implications;
- synthesis connecting the reading to the weekly theme.

Adapt question coverage to the source; do not force empirical-method questions onto conceptual readings or a theme connection that the source does not support. Each question must require explanation, comparison, interpretation, or synthesis, and must be answerable from the source.

Answers must be analytically substantive, not one-line keys. Use bullet points to explain the claim, the source's reasoning, relevant evidence, and meaningful conditions, limitations, or implications where supported. Include precise PDF page references where verifiable. Explain the relationship to the weekly theme, marking interpretation as such. Do not overstate evidence or turn an implication into an explicit finding.

Before finalizing, replace any item that merely repeats a heading or asks for an isolated fact. Check that all 10 questions together assess the central argument and key dependencies, that answer points explain why, and that references support the specific claims attached to them.

## Source readability and page references

- Use the PDF as the source of truth. Preserve important terminology and explain it plainly.
- If text is scanned, garbled, or unreadable, use available OCR or visual page inspection where appropriate. Clearly tell the user outside the document if any material could not be read reliably.
- Omit uncertain page-specific claims and references rather than guessing. Do not put process disclaimers, provenance boilerplate, or OCR-method boilerplate inside the DOCX.
- Never fabricate a generic page-reference disclaimer to fill the section. Include only page references that can be verified from the source.

## Final deliverable

- Final output format is DOCX: create one polished Word file containing all readings and sections. Do not create a PDF as the deliverable unless explicitly requested.
- Name it `Week X Reading Note.docx`, replacing `X` with the known course week number.
- Use 12 pt body text, single line spacing, and bullets for all answer points. Headings may be larger.
- Set Chinese text in 宋体 (SimSun) and English text in Times New Roman. Verify both scripts display correctly in Word.
- Save the file in the current project or the output location the user specifies. Provide a direct downloadable link after verifying the DOCX exists and is readable.
- Keep any notes about unreadable source material outside the Word document.
