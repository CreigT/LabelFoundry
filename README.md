# LabelFoundry

Public showcase for LabelFoundry: a synthetic cybersecurity training data pipeline.

**All generation code, quality gates, and configuration are private.**  
The complete system lives in a private repository accessible only to the owner.

## What this public repository contains
- Example source documents (NIST CSF, CISA, MITRE) used as inputs for grounded generation.
- High-level description of the approach.
- Link to the reviewed Hugging Face dataset.

No code or generated data is published here.

## Reviewed dataset (Hugging Face)

LabelFoundry v0.1 (gated):
https://huggingface.co/datasets/TcCreig/labelfoundry-soc-threat-descriptions

49 synthetic SOC incident descriptions (25 phishing, 24 ransomware).
Access is gated: you request it on Hugging Face and the owner approves requests by hand.

## Early access

Paid early access: https://labelfoundry-early-access.vercel.app

## Approach (high-level only)
1. Ingest cybersecurity source documents.
2. Generate QA pairs with a local LLM.
3. Apply quality checks.
4. Curate and release selected records.

No implementation details, source code, or configuration files are published here.

## Example source documents
The `data/sources/` folder contains public-domain style example documents only. They do not include any proprietary logic.

## SECURE

- Public repository contains no generation code, prompts, quality-gate implementation, or private configuration.
- Released dataset is gated on Hugging Face; owner approves access manually.
- Synthetic records are for defensive training and analysis only; they are not real incidents and do not prove model robustness.
- Source documents are public-domain style examples.

## VERIFY

Verification is evidence of the public boundary, not claims about private quality gates.

- Confirm no generation code or private config exists in this repository.
- Confirm the Hugging Face dataset remains gated and requires manual approval.
- Confirm the released set matches the stated count and categories (49 records).
- Confirm `data/sources/` contains only example documents.

See `docs/VERIFY_WALKTHROUGH.md` for the concrete check.

## DOCUMENT

- This README is the public summary.
- Full operational card: `docs/OPERATIONAL_CARD.md`
- Verification walkthrough: `docs/VERIFY_WALKTHROUGH.md`
- Documentation defines the public trust boundary; generation logic stays private.

---

Developed by Terrence Creig  
Sponsored by CREIGNIFICENT LLC

## Relevance to secure systems / edge / defense
Synthetic cyber data is useful for testing detection and defensive analysis workflows without disclosing real incidents. This is not proof of model robustness.
