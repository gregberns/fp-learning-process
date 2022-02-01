---
title: Sum Type
---

A Sum Type is an [[Algebraic Data Type]] that can be used to represent "this or that" type of structure. "Or" is the key word - the type only contains one of the values.

---

For example, the `Option` or `Maybe` type can represent "Something Or Nothing":

```
type Option =
	| Some(a)
	| None

let a = Some("foo")
let b = None

```

Another example is the `Either` type, which can represent `One thing Or Another thing`:

```
type Either =
	| Right(a)
	| Left(b)

let a = Right(1)
let b = Left("foo")
```

Option can be represented with Either (unit as the left or right), but not the other way around.

