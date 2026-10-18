# Prompt Engineering for Portfolio Building

## A good prompt has five parts

1. **Role** – "Act as a senior accounting data analytics instructor."
2. **Context** – course, dataset, audience, tools.
3. **Task** – one specific deliverable.
4. **Constraints** – length, tone, what not to do (no invented numbers).
5. **Output format** – table, markdown, code block.

## Example

> Act as a data analytics mentor. I analyzed a public dataset of monthly departmental budgets vs. actuals in Python. Write a README for my repo with sections: business question, data, approach, key findings, how to reproduce, limitations. Use placeholders like `[TODO: number]` where you lack facts. Output as Markdown.

## Tips

- Iterate: ask for a draft, then critique and refine.
- Provide real facts; verify every number the AI gives.
- Ask the AI to ask clarifying questions before writing.
- Save prompts that work in `.github/prompts/` for reuse.
- Never paste confidential client data into a chatbot.
