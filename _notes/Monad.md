---
title: Monad
---

[[I.Todo]] : Write blurb

---

A monad exists, generally when it implements `bind` and either `return` or `pure` (we'll use `pure`):

```
bind :: m a -> (a -> m b) -> m b
pure :: a -> m a
```

Monad and [[Functor]] type signatures are very similar, the significant difference is that the function passed in returns `b` in Functor's case an `m b` in Monads case.

Lets look at an example:

```
type Option = 
	| Some(a)
	| None
	
let bind: Option(a) => (a => Option(b)) => Option(b) = 
	m => f =>
		fun
		| Some(a) => f(a)
		| None => None
		
let pure: a => Option(a) =
	a => Some(a)
		
let a = bind(Some(1), x => pure(x + 1))
// output: Some(2)

let b = bind(None, x => pure(x + 1))
// output: None
```