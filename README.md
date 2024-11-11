# Como os Códigos de Tradução Foram Desenvolvidos

## Introdução
Os códigos apresentados utilizam a **API do Azure Translator**, parte dos serviços de IA da Microsoft, para realizar traduções automáticas. São dois exemplos principais: um focado na tradução de documentos `.docx` e outro na tradução de páginas da web. Aqui, explicamos como cada trecho do código foi estruturado e como funciona.

---

## Configuração Inicial
Antes de usar a API, é necessário configurar algumas variáveis principais:

- **subscription_key**: Sua chave de assinatura do serviço Azure Translator.
- **endpoint**: URL base do serviço (ex.: `https://api.cognitive.microsofttranslator.com`).
- **location**: Região do seu recurso no Azure.
- **language_destination**: Idioma para o qual o texto será traduzido (ex.: `pt-br`).

Essas variáveis são usadas em ambas as implementações.

### Exemplo:
```python
subscription_key = "SUA_CHAVE_API"
endpoint = 'https://api.cognitive.microsofttranslator.com'
location = "eastus"
language_destination = 'pt-br'
