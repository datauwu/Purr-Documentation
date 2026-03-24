# Types

Purr is statically typed with mostly inferred typing.

## Primitives
```typescript
let age: number = 25
let name: string = "Purr"
let flag: boolean = true
let nothing: null = null
```

## Type Inference
Types are inferred when possible, explicit annotations are optional.
```typescript
let x = 10        /* number */
let name = "Purr" /* string */
let flag = true   /* boolean */
```

## Union Types
A value can be one of several types.
```typescript
let a: number | string = 42      /* ok */
let b: number | string = "hello" /* ok */
```

And narrowing before use:
```typescript
let value: number | string = 42
if value is number {
    /* value is number here */
}
if value is string {
    /* value is string here */
}
```

> **Warning:** Using a union type without narrowing first may result in a compiler error.

## Nullable
A type followed by `?` means the value can be `null`.
```typescript
let name: string? = null   /* string or null */
let age: number? = 25      /* number or null */
```

## The `any` Type
`any` bypasses type checking and is only valid when initialized from a boundary function returning `any`.
```typescript
/* boundary functions are external functions that return any */
let value: any = boundaryFunction()
```

> **Warning:** `any` is not a dynamic type. Purr is still statically typed, `any` is an escape hatch for boundary interoperability only. It cannot be assigned from regular values.

## Type Aliases
```typescript
typealias ID = number | string
typealias Callback = (string) -> null
```

## Container Types
Container element types must be explicit.
```typescript
let nums = []<number>
let map = {}<string, number>
/* OR */
let nums2: array<number> = []
let map2: dict<string, number> = {}
```

## Type Checking
Narrow a union type at runtime using `is`.
```typescript
let x: number | string = 42
if x is number {
    print("it's a number")
}
```

[Link to next page: Operators](./operators.md)
