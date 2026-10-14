# Taiwanese English Checker · 台式英文抓蟲器

[繁體中文](README.md) | English

> Paste your English email, and AI points out the "Taiwanese English" (Chinglish) in it — what sounds off to native readers, why, and a natural rewrite.
> An AI agent skill (`SKILL.md`) that targets 30 patterns even good English writers use without realizing they are "Taiwanese English".

**👉 Landing page & free online try-out: https://wilsonaimaster.github.io/taiwanese-english-checker/**

## Why

Your email may be grammatically fine and still sound strange — or even rude — to an international client:

- `Look forward to hear from you.` — the "to" is a preposition; it needs "hearing".
- `Please be noted that…` — should be "Please note that…".
- `Please revert to me.` may confuse US and European readers.
- `The goods will ship on 03/04.` A client in Europe will read it as April 3.

Generic AI rewriting fixes your text but doesn't tell you **why**, so you repeat the same mistakes. This skill checks your writing the way a teacher would: every issue gets a severity level, a one-line reason, and a rule number, plus one habit worth remembering.

## Example

See [examples/client-email.md](examples/client-email.md) (explanations in Traditional Chinese).

The skill explains in the user's language: ask in English and you get English explanations.

## The 30 rules

Four groups: tone & politeness, direct translation from Chinese, common grammar slips, and business email habits (dates, currency, "revert", "Dear Sir"…). Full list: [references/rules.md](references/rules.md) (in Traditional Chinese, with English examples).

## 7 scenario packs

Beyond client emails, the skill adds scenario-specific rules on top of the 30 general ones: job hunting (J), workplace communication (W), presentations (P), cross-border e-commerce (E), academic writing (A), social media (S), and travel (T). See [references/scenarios/](references/scenarios/). Just tell the AI what the text is ("this is my cover letter"), or let it detect the scenario.

## Install

**Claude Code**

```bash
git clone https://github.com/WilsonAImaster/taiwanese-english-checker ~/.claude/skills/taiwanese-english-checker
```

**Other agents that support SKILL.md**: put the folder in that tool's skills directory.

**ChatGPT / Claude / Gemini (web)**: paste `SKILL.md` and `references/rules.md` into a Project or custom instructions.

## About

Built by Wilson, an English teacher of 16 years who explores how AI can make English actually useful at work. Found a wrong rule or a pattern we missed? [Open an issue](https://github.com/WilsonAImaster/taiwanese-english-checker/issues).

More AI tool tests: [Website](https://wilsonaienglish.com/) · [YouTube](https://www.youtube.com/@WilsonAILab) · [Skool](https://www.skool.com/wilson-9076) · [Instagram](https://www.instagram.com/wilsonailab/) · [Threads](https://www.threads.com/@wilsonailab)

## License

MIT
