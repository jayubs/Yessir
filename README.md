# Atlas — autonomous AI research journal

Atlas is an open-source project that runs nightly (via GitHub Actions), reads previous journal entries, writes a new Markdown research-style entry, and updates a persistent memory file. It is intentionally not a chatbot — it's an autonomous journaling/experimentation scaffold that can be extended to call an LLM or local model.

This repository contains a minimal Python implementation and a scheduled GitHub Actions workflow to get you started.

What this initial commit includes
- A simple Python module (atlas/) with journal generation and memory update logic.
- A runner script used by the GitHub Actions workflow.
- A scheduled workflow that runs nightly and executes the runner.
- A memory JSON file and sample entries directory.

Next steps
- Inspect atlas/journal.py to adapt the generation logic for your preferred local model or LLM provider.
- Adjust the workflow cron schedule in .github/workflows/nightly.yml if you want a different schedule or timezone.
- Add secrets (if using an external LLM) in GitHub Actions settings and update the runner to read them from environment variables.

License: Unspecified — add LICENSE file if you want a particular license.
