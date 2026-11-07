# LabelFoundry Operational Card
**Synthetic cybersecurity training data pipeline**  
Sponsored by CREIGNIFICENT LLC · Status: Public showcase; full generation system private

## Purpose
Produce grounded, curated synthetic cybersecurity examples (SOC incident descriptions, QA pairs) for defensive training and analysis without exposing real incidents or proprietary generation logic.

## Trust Boundaries
- Public repo contains only example source documents and high-level description.
- All generation code, quality gates, prompts, and configuration live in a private repository.
- Released data is gated on Hugging Face; owner approves access by hand.
- No raw generation outputs or private logic are published here.
- Synthetic data is for testing defensive workflows; it is not proof of model robustness or real incident fidelity.

## Current Enforcement / Release (v0.1)
- 49 synthetic SOC incident descriptions (25 phishing, 24 ransomware).
- Gated Hugging Face dataset: https://huggingface.co/datasets/TcCreig/labelfoundry-soc-threat-descriptions
- Access requires manual owner approval.
- Early access page: https://labelfoundry-early-access.vercel.app

## Explicit Non-Goals (current)
- Does not publish generation code or quality-gate implementation.
- Does not claim the synthetic records match real incident distributions.
- Does not auto-approve Hugging Face access requests.
- Does not expose private pipeline configuration.

## Verification Points
1. Public repo contains no generation code, prompts, or private config.
2. Hugging Face dataset is gated and requires manual approval.
3. Released records are limited to the stated curated set (49 examples).
4. Source documents in `data/sources/` are public-domain style examples only.

## Next Secure Step
Document the quality-gate criteria (without exposing implementation) in the private system and add a short verification note for any future public release that confirms schema and curation bounds.
