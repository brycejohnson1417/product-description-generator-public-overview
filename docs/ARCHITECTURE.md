# Architecture Diagram

```mermaid
flowchart LR
  User["Operator"]
  Input["Structured product input"]
  Upload["Synthetic document upload"]
  Parser["Parsing and extraction"]
  Normalize["Normalized product facts"]
  Rules["Tone and guardrail rules"]
  Generate["AI draft generation"]
  Review["Human review workspace"]
  Export["Approved copy export"]

  User --> Input
  User --> Upload
  Upload --> Parser
  Parser --> Normalize
  Input --> Normalize
  Normalize --> Rules
  Rules --> Generate
  Generate --> Review
  Review --> Export
```

## Public Boundary

- Source inputs and generated drafts are separate.
- Product facts come from structured inputs, not model guesses.
- The AI service drafts copy, but the review step decides what is approved.
- Public examples use synthetic products and synthetic lab-style documents only.

