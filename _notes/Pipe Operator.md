# Pipe Operator

The operator applies the left value to the function on the right as the last parameter.

```
let add: int => int => int = a => b => a + b

let five = 3 |> add(2)
// output: 5

// These expressions are equivalent
add(2, 3)
3 |> add(2)

```