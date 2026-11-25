---
name: document-skill
description: Add or update a skill in this skills repository, including its instructions, supporting files, and catalog entry.
---

# Document a skill

Create a skill that another person can find, understand, and use independently. Preserve the requested behavior and scope.

- Inspect the repository's README and existing skills for current conventions. Place each skill in `skills/<skill-name>/SKILL.md`, with a lowercase, hyphenated folder name matching the frontmatter `name`.
- Start `SKILL.md` with YAML frontmatter containing `name` and a concise `description` of what the skill does and when it applies. Follow it with focused Markdown instructions for the agent: purpose, decision criteria, essential steps, and genuine constraints.
- Keep the entry point self-contained and brief. Add `references/`, `scripts/`, or `assets/` only when useful; link to resources from the instructions and use relative paths. Avoid machine-specific paths, private information, and assumptions about installed tools or credentials.
- Update the root README's skill list with a short description and link. Keep installation instructions accurate for the repository's actual paths and default branch.
- Check that the folder and name match, frontmatter parses, links and resources resolve, and scripts work if included. If a skill validator is available, run it. Review the instructions against the user's request; a format check alone cannot verify their usefulness.
