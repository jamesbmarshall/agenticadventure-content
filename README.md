# Agentic Adventure — Content

This repository contains the educational content for [Agentic Adventure](https://github.com/jamesbmarshall/agenticadventure), a gamified learning platform for Microsoft Partners exploring AI, agentic AI, and building service capabilities.

The content is written in [MDX](https://mdxjs.com/) (Markdown with JSX components) and is pulled into the main site at build time.

## Structure

```
advisory/           Guides for teams starting their AI journey
professional/       Hands-on implementation and delivery guides
managed/            Advanced operational and managed service guides
paths/              Curated learning path definitions (JSON)
```

## Contributing

We welcome contributions. Whether you're fixing a typo, improving an explanation, or proposing a new guide, here's how to get involved.

### Editing an existing guide

1. Find the MDX file you want to edit (or use the "Edit this page" link on the site).
2. Fork this repository.
3. Make your changes.
4. Submit a pull request with a short description of what you changed and why.

### Writing a new guide

New guides are MDX files placed in the appropriate tier directory. Every guide needs this frontmatter at the top:

```yaml
---
title: "Your Guide Title"
description: "A one-sentence summary, under 160 characters."
tier: advisory | professional | managed
tags: ["tag-one", "tag-two"]
difficulty: 1-5
xp: 75 | 100 | 125 | 150 | 175
order: 1
author: "Your Name"
publishedAt: "YYYY-MM-DD"
featured: false
---
```

### Writing style

- **British English** throughout (colour, organise, behaviour).
- **No em dashes** (—). Use commas, semicolons, or colons instead.
- **Avoid AI clichés**: don't use "dive into", "leverage", "unlock", "empower", "harness", "cutting-edge", or "revolutionary".
- **Tone**: warm, practical, encouraging. Write like a colleague sharing field notes, not a textbook.
- **Audience**: Microsoft Partners — consultants, architects, developers, and practice leads.

For full writing guidelines, see the copywriter agent instructions in the main repository.

### Available MDX components

You can use these components inside guide content:

- `<QuestObjective completed={false}>Objective text</QuestObjective>` — learning outcome
- `<Callout type="info|warning|tip" title="Optional Title">Content</Callout>` — highlighted aside
- `<BillOfMaterials items={[{name: "Item", description: "Desc", required: true, link: "url"}]} />` — resource list
- `<LinkCard href="url" title="Title" description="Desc" />` — external link card

Plus standard Markdown: headings, lists, tables, code blocks, bold, italic, and links.

## Licence

Content is provided for educational purposes. See the main repository for licence details.
