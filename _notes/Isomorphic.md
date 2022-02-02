---
title: Isomorphic
---

If two types are isomorphic, there exists a mapping between the types, so that they can be mapped from `A` to `B` and back to `A` with no data lost.

---

For example:

```
type Bool = True | False
type Foo = Bar | Baz

let boolToFoo =
	fun
	| True => Bar
	| False => Baz
	
let fooToBool = 
	fun
	| Bar => True
	| Baz => False
	
let a = boolToFoo(fooToBool(Bar))
// output: Bar

let b = fooToBool(boolToFoo(False))
// output: False

// So 

```

## Category Theory

In Category Theory, category `A` must be isomorphic over itself via the [[Identity Function]] (`id`).

```
A == id(A)
```

Also there are situations when two categories are isomorphic to each other. (Add Details: What is it called when two categories are isomorphic to each other) When this is the case, there can be benefits.