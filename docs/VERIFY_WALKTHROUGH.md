# VERIFY Walkthrough — Public Release Bounds

**Goal:** Confirm the public repository does not leak generation logic and that released data remains gated and bounded.

## Steps
1. Clone or browse the public LabelFoundry repository.
2. Confirm no Python/generation scripts, prompt templates, or configuration files for the pipeline are present.
3. Check `data/sources/` — only example public-domain style documents.
4. Visit the Hugging Face dataset link. Confirm access is gated and requires a request + owner approval.
5. Confirm the README states the exact count (49 records) and categories.

## Pass Criteria
- No generation code or private config in the public repo.
- Dataset remains gated with manual approval.
- Public description matches the actual released set.

## Fail Criteria
- Generation code or prompts appear in the public repo.
- Dataset becomes public without gating.
- Undocumented records are released.

This verifies the public boundary. Full quality-gate verification stays in the private system.
