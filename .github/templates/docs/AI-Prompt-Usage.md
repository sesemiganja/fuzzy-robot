# Using the AI Prompt Template

Where to edit:
- For system-level behavior, edit: src/app/api/chat/route.ts
- For prompt files or examples, add or update .github/templates/ai_prompt_template.md and docs/AI-Prompt-Usage.md

Example: Create a README section
1. Open .github/templates/ai_prompt_template.md and fill:
   - Persona: expert developer, friendly
   - Task: Draft 120–150 word README installation section
   - Context: Node 18, Yarn, project uses Thesys C1
   - Format: 3 bullets (install, commands, troubleshooting)
   - Constraints: one example command, no >10-line code blocks
2. Paste final output into README.md or docs/.

Model verification:
- This repo includes a verification workflow that checks the Thesys model used in code. Keep src/app/api/ask/route.ts (or chat/route.ts) model names up to date and add THESYS_API_KEY secret to Actions if using the included workflow.

Tip:
- Always include at least one few-shot example inside "Constraints / Examples" to get consistent outputs.
