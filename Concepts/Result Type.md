# Result Type

`Result` is used to represent "Either a thing succeded with a value or failed with an error".

The `Result` type is a variant of the [[Either Type | `Either` type]], which is a [[Sum Type]]. `Result` is more specific (more powerful, less general), `Either` is more general, less powerful. 

Where `Either` has a `Right` and `Left`, `Result` has a success (`Ok`) and failure (`Error`) cases.

```
type Result =
	| Ok(a)
	| Error(e)
```

