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

# Description
Purr is a statically typed, multi-paradigm, bytecode-compiled language that is primarily executed on a C-based register VM, uses tracing garbage collection, and supports mostly inferred typing with explicit container element types. This repository contains the official documentation for Purr.
> Purr is still an experimental language, syntax and features may drastically change over time until the language is released.

# Philosophy

1. **Predictability** - clear syntax, unsurprising behaviour; follows the Principle of Least Astonishment.
2. **Performance** - static typing enables the compiler to do the hard work ahead of time, so the runtime executes with minimal guesswork.
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
