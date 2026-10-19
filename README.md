# Grok Bot MCQ Group Roles

5 specialized roles for a Grok Bot group that receives a photo of a multiple-choice question + options and returns only the correct answer with high accuracy and maximum speed.

## Roles
1. **VisionExtractor** — Accurate OCR and visual description only.
2. **SolverAlpha** — Primary independent solver.
3. **SolverBeta** — Alternative independent solver (different method).
4. **EvidenceCritic** — Verifies extraction fidelity and visual/logical evidence alignment.
5. **FinalAnswer** — Aggregates and outputs ONLY the answer letter. Zero extra text.

## Setup Instructions
1. Create 5 new Bots in Grok Bot.
2. Name them exactly as above (or similar).
3. Paste the full content of each corresponding `.md` file into the Bot's description / standing instructions (the operational role description).
4. Create a group chat and add all 5 Bots.
5. When you have a photo question, post the image in the group (optionally with a short message like "Analyze").
6. The bots will collaborate; FinalAnswer will reply with only the answer (e.g. `B`).

## Best Practices Applied
- Specialized narrow roles (official Grok Bot guidance).
- Parallel independent analysis for diversity (reduces cascade errors).
- Visual evidence alignment (EAGLE-style grounding).
- Strict output contracts for speed and zero fluff.
- Majority + evidence consistency for decision protocol (research-backed for MCQ/reasoning).

## Files
- [VisionExtractor.md](VisionExtractor.md)
- [SolverAlpha.md](SolverAlpha.md)
- [SolverBeta.md](SolverBeta.md)
- [EvidenceCritic.md](EvidenceCritic.md)
- [FinalAnswer.md](FinalAnswer.md)

Download individual files or clone the repo.

Raw links example: https://raw.githubusercontent.com/unhexx/grok-bot-mcq-group-roles/main/FinalAnswer.md
