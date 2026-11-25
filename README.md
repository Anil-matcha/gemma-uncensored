# Gemma Abliterated API with Muapi

Use Muapi's hosted Gemma 4 abliterated variants through a single API key. This guide compares the three Muapi model IDs and includes cURL and Python examples for async requests.

## Related Projects

- [Muapi Uncensored AI API guide](https://github.com/Anil-matcha/Uncensored-AI-API) — broader API setup and examples for Muapi's abliterated LLM endpoints.
- [Awesome Abliterated LLMs](https://github.com/Anil-matcha/awesome-abliterated-llms) — model comparison and evaluation notes.
- [Open Generative AI](https://github.com/Anil-matcha/Open-Generative-AI) — a creative AI workspace connected to Muapi.

## Muapi Gemma routes

| Model | Muapi endpoint |
|---|---|
| Gemma 4 26B A4B Abliterated | **gemma-4-26b-a4b-abliterated** |
| Gemma 4 31B Gembrain Abliterated | **gemma-4-31b-gembrain-abliterated** |
| Gemma 4 31B SDFT Abliterated | **gemma-4-31b-sdft-abliterated** |

The word “uncensored” in this repository name is a search label, not a guarantee about every route or response. Muapi identifies these variants as abliterated; behavior can vary by model and prompt. Follow Muapi's terms and applicable law.

## Quick start

Create a key at [Muapi API Keys](https://muapi.ai/access-keys), then set it in your shell:

~~~bash
export MUAPI_KEY="your-muapi-key"
~~~

Submit a prompt to the 26B A4B route:

~~~bash
curl -X POST https://api.muapi.ai/api/v1/gemma-4-26b-a4b-abliterated \
  -H "x-api-key: $MUAPI_KEY" \
  -H "Content-Type: application/json" \
  -d '{"prompt":"Summarize the design principles behind a well-tested API."}'
~~~

Poll the returned request:

~~~bash
curl "https://api.muapi.ai/api/v1/predictions/REQUEST_ID/result" \
  -H "x-api-key: $MUAPI_KEY"
~~~

The other variants use the endpoint IDs in the table. The [Gemma Abliterated API page](https://muapi.ai/gemma-abliterated-api) has current request details, availability, and pricing.

## Python example

Requires Python 3.9+ and **requests**.

~~~bash
python -m pip install -r requirements.txt
python examples/submit.py "Explain the difference between precision and recall."
python examples/submit.py --model gemma-4-31b-sdft-abliterated "Give a concise code review checklist."
~~~

## Links

- [Gemma Abliterated API on Muapi](https://muapi.ai/gemma-abliterated-api)
- [Muapi API reference](https://muapi.ai/docs/api-reference)
- [Create or manage an API key](https://muapi.ai/access-keys)
- [Muapi](https://muapi.ai)

Model availability, request fields, and pricing can change. Confirm them on the live Muapi page.
