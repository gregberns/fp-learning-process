---
title: <Interface Notes>
---

A note interface $I$ describes a set of properties and behaviors that a note $n$ should implement. 

## Explication

If there exists a link from $n$ to $I$, $n$ is said to *implement* $I$. In other words, the author of $n$ has committed to write $n$ in a manner satisfying the requirements defined by $I$. 

Additionally:
- $I$ cannot implement another interface.
- $n$ can implement any number of interfaces.
- Note interface names must follow the [[<Note Naming Conventions>|note naming conventions for interface notes]]

It is up to authors and maintainers to ensure that their notes truly satisfy the requirements of the interfaces their notes implement.

## Template

Use this [[<Interface Note Template>|template]] to create notes of this type.

## Why note interfaces?

- Interfaces allow authors to **declare design goals** for their notes ahead of time. This facilitates:
	-	Clear writing goals for the author.
	-	Objective rubric for editing/revision for collaborators.
	-	Communicative intent metadata attached to the note for the reader.
-	Interfaces semantically label links to from notes them as `n implements I` relationships, helping the reader.
-	Interfaces allow for ad-hoc organization for a knowledge mangagement system. 
	-	Circumvents `"Let's Think of a Perfect Structure for our System Before We Start Writing!"`-Syndrome.

