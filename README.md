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

---

Developed by Terrence Creig  
Sponsored by CREIGNIFICENT LLC
