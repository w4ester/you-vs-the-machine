# You vs. the Machine — The Reading Race

An offline-friendly, zero-dependency, single-page interactive thought experiment about human reading volume and published LLM pretraining-token counts.

## Play locally

Open `index.html` in any modern browser. No build step is required.

## Publish to GitHub Pages

1. Create a new **public** GitHub repository named `you-vs-the-machine`.
2. Upload `index.html` and `README.md` to the **root** of the default `main` branch.
3. Go to **Settings → Pages → Build and deployment**, select **Deploy from a branch**, then choose `main` and `/(root)`, and **Save**.
4. The URL should be `https://YOUR_USERNAME.github.io/you-vs-the-machine/` after GitHub Pages completes deployment.

## Math

`equivalent_words = trillion_tokens * 10^12 * 0.75`

`annual_words = pages_per_day * words_per_page * reading_days_per_week * 52`

`years = equivalent_words / annual_words`

`lifetimes = years / 80`

This estimates amount of *token exposure*, **not** unique material, comprehension, or memory. The token-to-word rate is an approximation for English text and is not a proper universal conversion of multimodal training data.

## References

- DeepSeek-V3 reported 14.8T pretraining tokens: https://github.com/deepseek-ai/DeepSeek-V3
- Qwen3 reported approximately 36T training tokens: https://qwenlm.github.io/blog/qwen3/
- Llama 3.1 reports >15T training tokens: https://ai.meta.com/blog/meta-llama-3-1/

The Llama 3.1 15T setting is deliberately a **lower bound**. The custom setting is hypothetical, not a claim about a proprietary model.

No analytics, cookies, external scripts, or backend. URL query parameters store shareable user settings.
