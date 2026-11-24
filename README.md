# voice-api-demos
Demos da API de voz

## Segredos

Este repo e publico. Nunca commite chaves, tokens, senhas SIP, IPs internos ou numeros de clientes.
Use variaveis de ambiente e um `.env` local (ja ignorado); deixe so um `.env.example` com placeholders.

O gitleaks roda no CI em todo push e PR e falha se achar segredo. Para checar antes do commit:

```sh
brew install gitleaks pre-commit
pre-commit install
gitleaks git --config .gitleaks.toml .
```
