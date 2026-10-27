# releases/

`python prepare_hf_release.py --version X.Y.Z` builds `releases/vX.Y.Z/` here on your computer:

- `train.jsonl`, `validation.jsonl`, `test.jsonl` (80/10/10 random split, fixed seed)
- `README.md` - dataset card draft (license is a TODO until a license is chosen)
- `manifest.json` - record counts, SHA-256 hashes, source file list, generator settings, git commit

It also adds an entry to `releases/CHANGELOG.md`.

The release folders are ignored by git and nothing is uploaded to Hugging Face.
Publishing needs Terrence Creig's approval.

---

Developed by Terrence Creig
Sponsored by CREIGNIFICENT LLC
