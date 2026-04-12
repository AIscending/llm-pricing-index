# LLM Pricing Index

Monthly pricing data for 20+ AI/LLM models, tracked and updated automatically.

**[View the full interactive index →](https://aiscending.com/ai-pricing-index/)**

## What's Included

- **22 models** across 4 categories: Frontier, Efficiency, Reasoning, Open Source
- **Price per 1M tokens** (prompt, completion, and blended)
- **Context window sizes**
- **Composite indices**: AI CPI (cost pressure index) and Budget Index
- **Monthly snapshots** starting April 2026

## Data Source

Pricing is pulled from the [OpenRouter API](https://openrouter.ai/docs#models) on the 1st of each month. OpenRouter aggregates pricing across providers, giving a standardized view of what each model actually costs.

## Files

| File | Description |
|------|-------------|
| `data/pricing_current.json` | Latest month's full pricing data |
| `data/pricing_history.json` | All historical snapshots |
| `data/models.csv` | Current prices in CSV format for spreadsheet use |

## Sample Data

```json
{
  "model_id": "openai/gpt-4o",
  "display_name": "GPT-4o",
  "provider": "OpenAI",
  "category": "frontier",
  "price_prompt_per_1m": 2.5,
  "price_completion_per_1m": 10.0,
  "price_blended_per_1m": 4.375,
  "context_length": 128000
}
```

## Categories

- **Frontier**: GPT-4o, Claude Sonnet 4, Gemini 2.5 Pro — highest capability, highest cost
- **Efficiency**: GPT-4o Mini, Gemini 2.0 Flash, Mistral Small — best price-to-performance
- **Reasoning**: o3 Mini, DeepSeek R1, Gemini 2.5 Flash Thinking — chain-of-thought models
- **Open Source**: Llama 4 Scout, Llama 3.3 70B, Qwen — self-hostable, lowest cost via API

## Composite Indices

**AI CPI (Cost Pressure Index)**: Weighted average cost across all tracked models. Measures overall market pricing direction.

**Budget Index**: Ratio of efficiency-tier pricing to frontier-tier pricing. Lower = bigger savings from choosing efficient models.

## Updates

Data refreshes automatically on the 1st of each month. Historical snapshots are preserved.

## Usage

This data is free to use in blog posts, research, tools, and applications.

**Attribution is required.** Please link to the source:

```
Data from AIscending LLM Pricing Index
https://aiscending.com/ai-pricing-index/
```

See [LICENSE](LICENSE) for full terms.

## About

Built and maintained by [AIscending](https://aiscending.com) — practical AI guidance for small business owners and solopreneurs. No hype, no jargon.

Questions? Contact sage@aiscending.com
