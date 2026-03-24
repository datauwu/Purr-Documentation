# Purr
Write it your way. No hairballs.
```typescript
struct Point { x: number; y: number }

class Printer {
    public function print(p: Point) {
        print(f"Hello from ({p.x}, {p.y})!")
    }
}

const transform = function(p: Point) -> Point {
    return Point { x: p.x + 1; y: p.y + 1 }
}

const p = transform(Point { x: 0; y: 0 })
new Printer().print(p)
```

# Warning
Purr is still an experimental language, syntax and features may drastically change over time until the language is released.

# Description
Purr is a statically typed, multi-paradigm, bytecode-compiled language that executes on a C-based register VM, uses tracing garbage collection, and supports mostly inferred typing with explicit container element types. This repository contains the official documentation for Purr.

# Philosophy

1. **Predictability** - clear syntax, unsurprising behaviour; follows the Principle of Least Astonishment.
2. **Performance** - programs run on a C-based register VM with a design that reduces the need for JIT compilation and heavy GC checks.
3. **Approachability** - emphasizes readable syntax, sensible defaults, and mostly inferred typing, allowing developers to write safe and efficient programs without excessive boilerplate.

# Paradigms

1. **Procedural**
2. **Structured**
3. **Object-oriented**
4. **Data-oriented**
5. **Functional**

# Learn More
- [Installation](docs/getting-started/installation.md)
- [Quick Tour](docs/getting-started/quick-tour.md)
