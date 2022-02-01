---
title: D.MOC Note
---
[[I.External]]


> A map of content (MOC) is a curated list of links, somewhat akin to a table of contents, that pulls together notes related to a topic.
> 
> MOCs are an alternative way to organize information that provides the flexibility of tags along with a less-rigid hierarchy of folders

[Source](https://www.ideasnotebook.com/Map+of+Content)

## Usage

Can be used to represent:
- Very broad concepts/topics that you want to link ideas together with, but that it doesn't make sense to write an article about. Ex: `Psychology`, `Philosophy`, `Programming Language` (You wouldn't write a full note about what a `Programming Language` is, but you might want a way to link `Python.md`, `Haskell.md`, `Ocaml.md`, etc to a common note.)
- Curated learning paths through conceptual terrain.
- Table-of-contents like hierarchy of ideas.

**Tip:** If you have a note named `{My MOC}`,  try adding `My MOC` to the `aliases:` front-matter field. This will allow Obsidian to pick up unlinked mentions of the note.

```md
<!-- {My MOC}.md -->
---
title: {My MOC}
aliases: [My MOC, Another Alias]
---
```


