# Quick Tour


## Variables
```typescript
let foo = 67
const barr = "purr"
```

## Functions
```typescript
function add(x: number, y: number) -> number {
    return x + y
}
```

## Classes
```typescript
class Animal {
    public name: string = ""
    public function printName() {
        print(f"{this.name}")
    }
}
```

## Structs
```typescript
struct Point { x: number; y: number }
const p = Point { x: 6; y: 7 }
```

## Enums
```typescript
enum Direction {
    North, South, East, West
}
```

## Error Handling
```typescript
try {
    throw "oops"
} catch const e: string {
    print(e)
}
```

## Imports
```typescript
import { add } from "math"
```


For full details see the [Language Reference](../language/variables.md).
