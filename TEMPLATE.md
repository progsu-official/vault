---
title: "Guide Title"
author:
  name: "Full Name"
  handle: "@progsu-handle"
readTime: "X min read"
publishDate: 2026-01-15T00:00:00.000Z
updated: 2026-01-15T00:00:00.000Z
tags: [tag-one, tag-two]
category: career
---

# guide title

One or two sentences. What this guide covers and who it's for. No fluff.

## quick start

If there's a clear action someone can take immediately, lead with it. If not, delete this section.

1. Step one
2. Step two
3. Step three

---

## vault structure

All guides live in category folders that mirror the wiki:

```
vault/
├── zero-to-hero/    roadmaps, internship/job search, getting started
├── career/          recruiting, resumes, offers, job search
├── technical/       leetcode, system design, interview prep
├── networking/      cold outreach, LinkedIn, warm intros
├── misc/            tools, productivity, everything else
└── template.md      this file
```

Create your `.md` file in the folder that matches your guide's topic. If it spans multiple categories, pick the primary one.

---

## frontmatter fields

Every guide must start with YAML frontmatter between `---` delimiters:

```yaml
---
title: "Your Guide Title"
author:
  name: "Full Name"
  handle: "@progsu-handle"
readTime: "8 min read"
publishDate: 2026-05-25T00:00:00.000Z
updated: 2026-05-25T00:00:00.000Z
tags: [career, resume, internship]
category: career
---
```

### field reference

- **title** (required): display title of the guide, plain sentence case
- **author.name** (required): your full name
- **author.handle** (required): your progsu username with `@`
- **readTime** (required): honest estimate, e.g. `"5 min read"`. count on ~200 words per minute
- **publishDate** (required): ISO 8601, set once and leave it
- **updated** (required): ISO 8601, update this every time you revise the guide
- **tags** (required): lowercase, hyphenated, 2-5 tags. these drive the knowledge graph
- **category** (required): one of `zero-to-hero`, `career`, `technical`, `networking`, `misc`

---

## headings

The wiki navigation and knowledge graph both generate from your headings. Use standard markdown:

```markdown
# main section

## major subsection

### minor subsection

#### detail
```

Do not use HTML heading tags. Do not skip levels (e.g. jumping from `#` to `###`).

### heading hierarchy in the sidebar

- `#` and `##` appear at the top level
- `###` is indented, smaller
- `####` is further indented, smallest

---

## cross-references and knowledge graph

This is an Obsidian vault. Use wikilinks to connect related guides:

```markdown
[[resume-guide]]
[[behavioral-questions]]
```

The wiki renders these as clickable links. The knowledge graph hero on the home page is built from these connections. The more accurately you link related guides, the more useful the graph becomes.

Link when:
- a concept in your guide has its own dedicated guide
- a reader would benefit from reading another guide alongside this one
- you reference a term or framework explained elsewhere in the vault

Do not link for the sake of linking. Every wikilink should be genuinely useful to the reader.

---

## tags

Tags are the second input to the knowledge graph, alongside wikilinks. Use them to describe what a guide is *about*, not just what category it falls in:

```yaml
tags: [resume, ats, formatting, career]
```

Tag guidelines:
- lowercase, hyphenated
- 2 to 5 tags per guide
- describe topics, not adjectives (`resume` not `important`)
- reuse existing tags rather than coining new ones

---

## callouts

Use Obsidian callout syntax for highlighted content:

```markdown
> [!tip]
> A helpful tip or shortcut worth calling out.

> [!warning]
> Something that commonly goes wrong.

> [!note]
> Additional context that doesn't fit inline.

> [!info]
> Background information the reader may want but doesn't need.
```

Use callouts sparingly. One or two per guide is plenty. If everything is highlighted, nothing is.

---

## standard formatting

### code blocks

Always specify the language:

````markdown
```bash
npm run dev
```

```python
def example():
    pass
```
````

### tables

```markdown
| column one | column two |
|------------|------------|
| data       | data       |
```

### lists

```markdown
- unordered item
- unordered item

1. ordered item
2. ordered item
```

### emphasis

```markdown
**bold** for key terms on first use
*italic* for titles, light emphasis
`inline code` for commands, filenames, variables
```

---

## file naming

- lowercase only
- hyphens for spaces
- descriptive, not generic

```
resume-guide.md          ✓
technical-interview-prep.md  ✓
behavioral-questions.md  ✓
Guide1.md                ✗
my guide.md              ✗
new-guide.md             ✗
```

---

## voice and tone

Writing for GSU students, many first-gen, many self-taught, many anxious about breaking into tech. They are smart but new.

- plain sentences, no jargon
- lowercase headlines
- lowercase sentence starts in paragraphs and lists too, but keep proper nouns, brand names, and acronyms capitalized (Google, LinkedIn, FAANG, SQL)
- frame everything as "here's how", not "you should already know"
- empty states and edge cases should encourage, not scold
- no exclamation points, no marketing voice, no emoji

When in doubt, cut the sentence. If it doesn't help the reader do something, it doesn't need to be there.

---

## updating an existing guide

1. Edit the file directly
2. Update the `updated` field in frontmatter to today's date
3. Commit with a clear message describing what changed and why
4. The wiki picks up the change automatically on the next deploy

---

## testing locally

Open the vault folder in Obsidian to preview your guide before pushing:

1. Open Obsidian
2. "Open folder as vault" and select the `vault/` directory
3. Your guide will render with wikilinks, callouts, and tags active
4. Check that wikilinks resolve to existing files

---

## checklist before pushing

- [ ] frontmatter complete with all required fields
- [ ] file in the correct category folder
- [ ] standard markdown headings only, no skipped levels
- [ ] wikilinks point to guides that exist
- [ ] 2 to 5 tags, lowercase and hyphenated
- [ ] `updated` date reflects today
- [ ] read it out loud once, cut anything that doesn't help the reader
