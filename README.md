# FileReview

FileReview is a public library of GitHub Copilot agent skills for reviewing PDFs
for inconsistencies. The skills guide Copilot through comparing statements
between paragraphs and comparing paragraph text with text embedded in figures,
scans, screenshots, and other images.

## Available skills

| Skill | Purpose |
| --- | --- |
| [`pdf-consistency-review`](.github/skills/pdf-consistency-review/SKILL.md) | Review a supplied PDF for conflicting or inconsistent statements, including text in images. |

## Use with GitHub Copilot

Use this repository with Copilot, or copy the skill's folder into the
`.github/skills/` directory of a repository where you use Copilot. In Copilot
Agent mode, provide the PDF and ask for a consistency review. For example:

> Review the attached PDF using the `pdf-consistency-review` skill. Also apply
> the rules in the `style-and-units-review` skill.

Additional rule skills can be added to `.github/skills/<skill-name>/SKILL.md`.
Ask Copilot to apply the relevant rule skill along with the PDF review skill;
the PDF review skill does not define or assume specialized domain rules.

Copilot's ability to read attachments and inspect image text depends on the
client and tools available in the session. The skill requires it to report
unreadable pages or images rather than imply they were fully reviewed.
