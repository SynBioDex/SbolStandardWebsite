# Adding a GenAI Tool

GenAI tools appear on the **Ecosystem → GenAI Tools** page. These are AI-powered assistants, models, or resources that help users understand or work with SBOL — for example, custom GPTs trained on the specification.

---

## Where the files live

```
content/genai-tools/
└── your-tool-slug/
    └── index.md
```

No image is needed — the cards are text-based.

---

## Step-by-step

1. Create a new folder inside `content/genai-tools/` (lowercase, hyphenated).
2. Add `index.md` with the front matter below.
3. That's it — no other files needed.

---

## Template

```markdown
---
title: "Your Tool Name"
summary: "Two or three sentences describing what the tool does and who it is for."
external_url: "https://link-to-the-tool.com"
platform: "ChatGPT"       # the platform the tool runs on, e.g. ChatGPT, HuggingFace
sbol_version: "3"         # "2", "3", or omit if not version-specific
---
```

> **Important:** Use `external_url`, not `url`. Hugo reserves `url` as the page's own address — using it here will cause a build error.

---

## Real example

`content/genai-tools/sbol3-gpt/index.md`

```markdown
---
title: "SBOL 3 GPT"
summary: "A custom ChatGPT assistant trained on the SBOL 3 specification and the pySBOL3 library. Ask it anything about SBOL 3 data models, syntax, and Python usage."
external_url: "https://chatgpt.com/g/g-FcRCPqKq6-sbol-3"
platform: "ChatGPT"
sbol_version: "3"
---
```

---

## Field reference

| Field | Required | Notes |
|---|---|---|
| `title` | Yes | Name of the tool, shown as the card heading |
| `summary` | Yes | Description shown on the card. Two or three sentences works well |
| `external_url` | Yes | The link users click to open the tool. Must be `external_url`, not `url` |
| `platform` | No | Shown as a badge on the card (e.g. `ChatGPT`, `HuggingFace`, `Notebook`) |
| `sbol_version` | No | Shown as a green `SBOL 2` or `SBOL 3` badge. Omit if not version-specific |

---

## Common mistakes

- **Using `url` instead of `external_url`** — Hugo treats `url` as the page's own path. If you use an `https://` URL there, the build will fail with an error about unsupported URL protocols.
- **Leaving `platform` blank** — the platform badge helps users quickly understand what environment the tool runs in. Always fill it in if you know it.
