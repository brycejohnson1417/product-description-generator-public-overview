# Prohibited Claims, Review, And Prompt Guardrails

## Prohibited Claims

The generator should avoid:

- Medical or treatment claims.
- Guaranteed effects.
- Unsupported potency statements.
- Statements not present in structured product inputs.
- Claims inferred only from a document image or filename.

## Human Review

Generated copy is a draft, not an approved final asset. A reviewer should check:

- Product name and format.
- Channel fit.
- Tone.
- Compliance-sensitive language.
- Whether every claim maps back to an approved input.

## Prompt Guardrails

Prompt construction should:

- Include only approved product facts.
- Separate facts from tone instructions.
- List prohibited claims explicitly.
- Ask for draft copy, not final approved copy.
- Preserve a review step before export.

