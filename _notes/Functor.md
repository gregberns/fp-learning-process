---
---

#	Functor

Haskell Functor signature: `Functor f => (a -> b) -> f a -> f b`

Where `f` is a Functor, `(a -> b)` is a function that transforms `a` to `b`, and takes an `f a` (Functor of type `a`) and returns an `f b` (Functor of `b`).

This is an example of a functor called `Option`, you'll also hear it referred to as the `maybe` data type. `Option` is an [[Algebraic Data Type| Algebraic Data Type or ADT]], specifically it is a [[Sum Type]].

```
type Option(a) =
	| Some(a)
	| None

let map: (a => b) => Option(a) => Option(b) = f =>
	fun
	| Some(a) => Some(f(a))
	| None => None

// Constructor usage
let a = Some(1);
let b = None;

// Functor has one function: `map`
let c = Option.map(x => x + 1, Some(1));
// output: Some(2)

let d = Option.map(x => x + 2, None)
// output: None
```

