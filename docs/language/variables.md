# Variables

Purr has two variable declarations: `let` and `const`.

## let
Mutable; the binding and its value can be reassigned.
```typescript
let x = 10
x = 20 /* works, btw # also works for comments too */
```

## const
Weakly immutable; the binding cannot be reassigned, but the contents of the value can still be mutated.
```typescript
const x = 10
x = 20 /* error */

const p = Point { x: 0; y: 0 }
p.x = 5 /* it works */
```

[Link to next page: Types](./types.md)
