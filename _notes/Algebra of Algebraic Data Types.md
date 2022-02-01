---
title: Counting the Values in a Type
---

## Counting the Values in a Type 

Possible values in a type

[This is a good overview](https://gist.github.com/gregberns/5e9da0c95a9a8d2b6338afe69310b945) on how types can be converted to an algebra which allows us to count the potential values or possibilities of a type.

---

`type Unit = Unit` - this is generally the type that represents 1 value. It is, and can only be one value.

`type Bool = True | False` can be two values: `True` or `False`. The quantity of values in type `Bool` are 2. 

`type Foo = Bar | Baz` is also 2 values, so if we created a mapping between `Bar` and `True`, and `Baz` and False, both data structures represent the same quantity of values (2). Because they can be mapped back and forth, this means they are [[Isomorphic|isomorphic]] - or no data is lost between the mapping.

This is helpful, because if you know `Foo` is isomorphic to `Bool`, and you know `Bool`s value count is 2, then you also know `Foo`s count is 2.