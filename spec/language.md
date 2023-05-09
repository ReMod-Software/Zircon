# Zircon

Zircon is a programming language designed as a Rust and Ruby hybrid, it borrows
the great tooling ideas of Rust while combining them with Ruby's ideas of
readability and syntax.

## Motivation
Ruby is a powerful and expressive language, however, with great power comes great responisibility. Despite being extremely powerful, it suffers because of so many options make it confusing for people to pick one. Rust on the other hand, is a language oriented for efficient systems, however, it is also very productive because of how it is designed. It has stellar tooling, docs, and standard library, something which Ruby utterly fails at. Zircon aims to combine best of both worlds, while being more high-level and also taking bits from other languages like TypeScript and Kotlin.

## Goals
- Provide Good DX and UX for the final output, including Hot Module Reload, Stellar Standard Library, Good Performance, and more
- Compile to JavaScript initially, but have a WASM (Browser & WASI-oriented) and Native Target via Cranelift
- Be Readable & Expressable like Ruby; Efficient and Productive as Rust
- Be Simple; all the complex magic happens in Standard Library, not core language

## Prior Art
- [Rust](https://rust-lang.org)
- [Ruby](https://ruby-lang.org)
- [TypeScript](https://typescriptlang.org)