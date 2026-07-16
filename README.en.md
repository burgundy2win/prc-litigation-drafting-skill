# PRC Civil Litigation Drafting & Evidence Skill

A Codex Skill for drafting, reviewing, and verifying civil-litigation documents and evidence packages in the context of PRC legal practice.

## Capabilities

- Draft, revise, and finalize civil defense briefs, civil complaints, and appraisal applications.
- Prepare evidence directories and civil evidence registers.
- Organize, merge, bookmark, consecutively paginate, and verify evidence PDFs.
- Conduct evidence-oriented review of DOCX files, PDFs, scans, chat records, payment records, and other electronic data.
- Flag factual or pagination gaps instead of presenting unverified matters as established facts.

## Design Principles

This Skill is not just a text generator. It maps claims, elements of defense, burdens of proof, and disputed issues to specific evidence, then follows a controlled sequence:

1. Define the evidence scope, grouping, numbering, and order.
2. Merge, correct, and consecutively paginate the evidence PDF.
3. Backfill the evidence directory, evidence register, and litigation-document footnotes.
4. Verify consistency across names, dates, amounts, entity information, page references, bookmarks, signatures, and seals.

When facts or evidence are incomplete, the Skill requires the working draft to use the marker `【To Be Confirmed】` rather than inventing content. For substantive review of existing legal Word documents, it recommends Track Changes and comments, with review metadata configured as the neutral label `Reviewing Attorney`.

## Repository Structure

```text
SKILL.md                              # Entry point and general workflow
references/defense-brief.md           # Civil defense-brief rules
references/complaint-and-appraisal.md # Civil complaint and appraisal-application rules
references/evidence-package.md        # Evidence-directory and evidence-package rules
agents/openai.yaml                    # Optional interface metadata
```

## Usage

Place the directory in your Codex Skills directory, then invoke it explicitly:

```text
$draft-defense-evidence Process this case's defense brief and evidence materials under the standard workflow.
```

You can also describe a task directly, such as “Prepare an evidence directory and merge the evidence PDFs under the standard workflow.” Always provide the materials for the current case, and have a qualified legal professional review and confirm the final work product.

## Privacy and Disclaimer

This public version removes personal names and machine-local paths. It provides workflow and document-organization rules only; it is not legal advice and does not replace independent professional judgment on case facts, evidence, applicable law, or procedural requirements.

中文说明：[README.md](README.md)
