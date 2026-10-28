# Huawei Cloud MaaS Calculator

A single-file, dependency-free web calculator for estimating the cost of Huawei Cloud MaaS models. Open the HTML file directly in a browser — no build step or server required.

## File

`Huawei Cloud MaaS Calculator-v1.03.html`

## Features

- **Price table** — context length, max input/output length, max CoT length, input/output type, and input / cached-input / output prices per model.
- **Cost Calculator** — enter input tokens, output tokens, cache hit rate, and the normal / night token split to estimate the cost per model.
- **Tokens Calculator** — enter a budget, cache hit rate, input/output token ratio, and the normal / night split to see how many input/output tokens each model can buy.
- **Night discount preview** — a toggle previews the night-discount prices in the main table.
- **Bilingual UI** — switch between Chinese and English with the `EN` / `中文` button.

## Models

- `GLM-5.2` — night discount 30% off (7-折)
- `GLM-5.3` — no night discount
- `DeepSeek-V4.1-Flash` — night discount 50% off (5-折)
- `DeepSeek-V4.1-Flash-1017` — same price and discount as `DeepSeek-V4.1-Flash`

Night discount applies during 21:00–08:00 Beijing time.

## Pricing Notes

- Prices are in **USD per million tokens** (list price).
- Models that support a cached-input price split input cost into normal / cached based on the hit rate.
- Normal input cost = input tokens × input price × (1 − hit rate)
- Cached input cost = input tokens × cached price × hit rate
- Output cost = output tokens × output price
