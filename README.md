# voice-api-demos
Fluke voice API demos

## Demos

- [`voice-ai-agent`](voice-ai-agent/): call a Brazilian number with an AI agent on the line over SIP (OpenAI Realtime, or any SIP-capable AI).

## Secrets

This repo is public. Never commit keys, tokens, SIP passwords, internal IPs or customer numbers.
Use environment variables and a local `.env` (already ignored); keep only a `.env.example` with placeholders.

gitleaks runs in CI on every push and PR and fails if it finds a secret. To check before committing:

```sh
brew install gitleaks pre-commit
pre-commit install
gitleaks git --config .gitleaks.toml .
```
