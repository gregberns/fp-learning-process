---
---

# Lenses

Lenses support accessing and modfying immutable data structures, especially nested data structures that would otherwise be difficult to access and modify. 

Lenses are a subset of [[Optics]].

```hs
data Lens a b = Lens (a -> b -> a) (a -> b)

get :: Lens a b -> a -> b
get (Lens _ g) = g

set :: Lens a b -> a -> b -> a
set (Lens f _) = f

// This is an example of a lens over a Tuple
first = Lens (\(_, b) x -> (x, b)) (\(a, _) -> a)
second = Lens (\(a, _) x -> (a, x)) (\(_, b) -> b)

```

