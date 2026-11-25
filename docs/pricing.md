# Pricing

The figures below are Muapi catalog rates per million tokens, checked on 2026-11-25. Input and output rates can differ. These values are a dated snapshot; verify the live Muapi page before budgeting.

| Model | Input / 1M | Output / 1M | Context | Input type |
|---|---:|---:|---:|---|
| <code>gemma-4-26b-a4b-abliterated</code> | $0.30 | $1.40 | 65K | Text |
| <code>gemma-4-31b-gembrain-abliterated</code> | $0.612 | $0.612 | 262K | Text + image |
| <code>gemma-4-31b-sdft-abliterated</code> | $0.612 | $0.612 | 262K | Text + image |

## Estimate a request

A rough estimate is:

```text
estimated cost = (input tokens × input rate + output tokens × output rate) ÷ 1,000,000
```

Actual charges depend on usage and Muapi's current billing rules. Check the response usage or cost fields and your Muapi dashboard for account totals.

## Price changes

Model availability, context limits, fields, and rates can change. Verify the live [Muapi model page](https://muapi.ai/gemma-abliterated-api) or the [Muapi catalog](https://muapi.ai/models).
