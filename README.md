# PromptSpace Prompts — 100 Free, Copy-Paste AI Prompts

<p align="center">
  <a href="https://www.promptspace.in"><img alt="PromptSpace" src="https://img.shields.io/badge/curated%20by-PromptSpace-emerald?style=for-the-badge"></a>
  <a href="LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge"></a>
  <a href="CONTRIBUTING.md"><img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-orange?style=for-the-badge"></a>
  <img alt="Prompts" src="https://img.shields.io/badge/prompts-100-teal?style=for-the-badge">
</p>

**100 curated, free AI prompts** across the models people actually use —
Midjourney, FLUX, Stable Diffusion, DALL·E, ChatGPT, Claude. Every prompt is
a plain `.md` file: title, tags, the exact prompt block, negative prompt +
settings where relevant, and a link back to the source on
[PromptSpace](https://www.promptspace.in).

No signup. No paywall. Fork it, grep it, ship it.

---

## 🚀 Why this repo exists

[PromptSpace](https://www.promptspace.in) hosts **5,000+ free AI prompts** on
the web. This repo is a **community-curated slice** you can:

- `git clone` and grep locally with `rg` / `fzf`.
- Feed into your own scripts, agents, or fine-tuning pipelines.
- Fork and extend with your own battle-tested prompts.
- Star to bookmark — new prompts land here monthly.

Every prompt links back to its canonical page on PromptSpace so you can see
the example output, remix it in-browser, or tune it with the free
[**Prompt Optimizer**](https://tools.promptspace.in/prompt-optimizer).

---

## 📂 Categories

| Folder                                              | Model / use case                     | Count |
| --------------------------------------------------- | ------------------------------------ | ----: |
| [`midjourney/`](./midjourney)                       | Midjourney v6/v7 image prompts       |    73 |
| [`flux/`](./flux)                                   | FLUX (dev + pro) photoreal + cinema  |    19 |
| [`stable-diffusion/`](./stable-diffusion)           | SDXL / SD 1.5 stylized + illustration |     4 |
| [`image/`](./image)                                 | Model-agnostic image prompts         |     4 |
| [`chatgpt/`](./chatgpt)                             | ChatGPT text prompts (open for PRs)  |     0 |
| [`claude/`](./claude)                               | Claude text prompts (open for PRs)   |     0 |

> **Note.** PromptSpace's public library is currently image-focused.
> The `chatgpt/` and `claude/` folders are seeded and open for community
> contributions — see [CONTRIBUTING.md](./CONTRIBUTING.md).

`index.json` at the repo root has structured metadata for every prompt
(`file`, `title`, `slug`, `tags`, `canonical_url`, `views`) — handy for
programmatic use.

---

## 🎨 Quick start

```bash
git clone https://github.com/<your-org>/promptspace-prompts.git
cd promptspace-prompts

# Browse
ls midjourney/ | head

# Fuzzy-find any prompt
grep -riE "portrait|cinematic" midjourney/

# Load metadata
jq '.prompts[0]' index.json
```

Each prompt file follows the same shape:

````markdown
# Prompt Title

**Category:** … · **Tags:** … · **Views on PromptSpace:** 3,515

> Curated from [PromptSpace](https://www.promptspace.in/prompt/<slug>).

![preview](https://cdn.promptspace.in/prompts/<id>.webp)

## Prompt
```text
<the full prompt, ready to paste>
```

## Negative Prompt / Settings / Tips
…

---
Source: [<title>](https://www.promptspace.in/prompt/<slug>) ·
Browse 5,000+ prompts at [promptspace.in](https://www.promptspace.in) ·
Optimize any prompt with the [Prompt Optimizer](https://tools.promptspace.in/prompt-optimizer).
````

---

## 🤝 Contribute

Have a killer prompt? PRs are welcome — one prompt per file, one file per PR.
Full guide: [CONTRIBUTING.md](./CONTRIBUTING.md).

Adding a prompt is three steps:

1. **Fork** this repo.
2. **Add** `your-slug.md` in the right folder (see [CONTRIBUTING.md](./CONTRIBUTING.md#template)).
3. **PR** with a short "why this prompt is good" note.

We review within 48 hours. If you're stuck, DM
[@promptspacein](https://twitter.com/promptspacein) on X.

---

## 🛠 Related PromptSpace tools

- **[Prompt Optimizer](https://tools.promptspace.in/prompt-optimizer)** — paste any prompt, get a tuned version for your target model. Free, no signup.
- **[Free Prompt Library](https://www.promptspace.in/free-ai-prompt-library)** — 5,000+ prompts, filter by style/model/tag.
- **[Blog](https://www.promptspace.in/blog)** — prompt-engineering tutorials + case studies.

---

## ⭐ Star history

<a href="https://www.star-history.com/#PromptSpace/promptspace-prompts&Date">
  <img alt="Star History" src="https://api.star-history.com/svg?repos=PromptSpace/promptspace-prompts&type=Date">
</a>

---

## 📜 License & attribution

MIT — see [LICENSE](./LICENSE).

Prompts curated from the public
[PromptSpace](https://www.promptspace.in) library.
If you republish, please keep the source link back to
`https://www.promptspace.in/prompt/<slug>` — this repo exists to grow the
free prompt commons, not to strip attribution.

Built with ❤️ by the [PromptSpace](https://www.promptspace.in) team and
contributors like you.
