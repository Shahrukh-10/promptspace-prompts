# Contributing to PromptSpace Prompts

Thanks for wanting to add to the free prompt commons! This repo is
deliberately low-ceremony: **one prompt per markdown file**, one PR per
prompt (or a small batch of related prompts).

## Ground rules

1. **Original or freely-licensed only.** Don't copy prompts from paywalled
   sources. Prompts you wrote yourself, or ones already public on
   [promptspace.in](https://www.promptspace.in), are perfect.
2. **It has to actually work.** Test it in the target model before opening
   the PR. Screenshots of the output in the PR description are a huge plus.
3. **Keep the palette clean.** No shock content, no impersonation, nothing
   the target model would refuse. If a prompt needs a jailbreak, it's not
   for this repo.
4. **One prompt = one file.** Makes them easy to grep, cite, and remix.

## Where does my prompt go?

| Folder                | Use for                                              |
| --------------------- | ---------------------------------------------------- |
| `midjourney/`         | Midjourney v6/v7 image prompts                       |
| `flux/`               | FLUX (dev/pro/schnell) — photoreal, cinematic        |
| `stable-diffusion/`   | SDXL, SD 1.5, Pony, illustrated styles               |
| `image/`              | Model-agnostic image prompts (work anywhere)         |
| `chatgpt/`            | ChatGPT text prompts (writing, code, analysis, etc.) |
| `claude/`             | Claude text prompts (long-form, agents, coding)      |

## File naming

- lowercase-kebab-case: `cinematic-cyberpunk-street.md`
- Slug should be human-readable and unique within the folder.
- Max 80 characters.

## <a id="template"></a> Template

Copy-paste this into your new `.md`, fill it in, delete the sections you
don't need.

````markdown
# Cinematic Cyberpunk Street

**Model:** Midjourney v7 · **Tags:** `cinematic`, `cyberpunk`, `street`, `neon`

> Short 1–2 line description of what this prompt does and when to reach for it.

## Prompt

```text
<the full prompt, exactly as you'd paste it, no ellipsis>
```

## Negative Prompt (optional)

```text
<negative prompt if applicable>
```

## Suggested Settings (optional)

- Aspect ratio: `--ar 16:9`
- Stylize: `--s 250`
- Model: `--v 7`

## How to Use (optional)

Any prep steps, chaining hints, or variations worth calling out.

## Tips (optional)

Failure modes, when it works best, common tweaks.

---
Contributed by [@yourhandle](https://github.com/yourhandle).
Inspired by / adapted from [PromptSpace](https://www.promptspace.in) — the
free AI prompt library.
````

## Also update `index.json`

Add a new entry so the metadata index stays in sync:

```json
{
  "file": "midjourney/cinematic-cyberpunk-street.md",
  "title": "Cinematic Cyberpunk Street",
  "slug": "cinematic-cyberpunk-street",
  "category_folder": "midjourney",
  "tags": ["cinematic", "cyberpunk", "street", "neon"],
  "model_hint": "midjourney",
  "canonical_url": "https://www.promptspace.in/prompt/cinematic-cyberpunk-street",
  "views": 0
}
```

(If your prompt isn't published on promptspace.in yet, either drop
`canonical_url` or point it to your PR URL. If you'd like the PromptSpace
team to publish it on the site as well, mention that in the PR description.)

## Review process

- Maintainers review within 48 hours (usually faster).
- Small tweaks (typos, tag adjustments, formatting) — we may commit directly
  and credit you in the merge commit.
- Structural changes (new folders, README rewrites, tooling) — open an
  issue first so we can align.

## Code of conduct

Be excellent to each other. No harassment, no doxxing, no NSFW targeting
real people. Maintainers reserve the right to close PRs or ban contributors
who don't follow this.

---

Questions? Ping [@promptspacein](https://twitter.com/promptspacein) on X, or
open a
[Discussion](https://github.com/PromptSpace/promptspace-prompts/discussions).
