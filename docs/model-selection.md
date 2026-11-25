# Choosing a Gemma route

This guide covers three hosted Gemma 4 endpoints. It separates the text-only 26B A4B route from the image-capable 31B variants and records their Muapi catalog limits and prices.

## Compare the current routes

| Route | Context | Input | Input / output per 1M tokens | Maximum output | Selection note |
|---|---:|---|---:|---:|---|
| <code>gemma-4-26b-a4b-abliterated</code> | 65K | Text | $0.30 / $1.40 | 16384 | Choose when text-only input and the 26B A4B route fit your workload. |
| <code>gemma-4-31b-gembrain-abliterated</code> | 262K | Text + image | $0.612 / $0.612 | 16384 | Choose when image input is needed and you want to evaluate the Gembrain variant. |
| <code>gemma-4-31b-sdft-abliterated</code> | 262K | Text + image | $0.612 / $0.612 | 32768 | Choose for creative or character-chat tasks, then review results against your own evaluation set. |

The table is a shortlist by documented interface, context, and price. It is not a quality ranking.

## A practical selection process

1. Start with input type. Use image_url only on a route whose Muapi schema lists image input.
2. Match the advertised context window to the total prompt size and leave room for the generated answer.
3. Set max_tokens to the output length your task needs; the cap varies by endpoint.
4. Estimate cost from expected input and output token counts using the separate rates.
5. For close choices, run the same prompts on each route and score them against your own criteria. This repository publishes no comparative benchmark scores.

## Model cards

- [Gemma 4 26B A4B Abliterated](models/gemma-4-26b-a4b-abliterated.md) — Choose when text-only input and the 26B A4B route fit your workload.
- [Gemma 4 31B Gembrain Abliterated](models/gemma-4-31b-gembrain-abliterated.md) — Choose when image input is needed and you want to evaluate the Gembrain variant.
- [Gemma 4 31B SDFT Abliterated](models/gemma-4-31b-sdft-abliterated.md) — Choose for creative or character-chat tasks, then review results against your own evaluation set.

Check the [Muapi live page](https://muapi.ai/gemma-abliterated-api) for current availability and pricing.
