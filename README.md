## Overview

The project structure is organized around different phases of the compiler:

```
src/
│
├── IR/
│   └── main.rs
│
├── codegen/
│   └── main.rs
│
├── lexer/
│   └── main.rs
│
├── main.rs
│
├── mod.rs
│
├── optimizer/
│   └── main.rs
│
├── parser/
│   └── main.rs
│
└── semantics/
    └── main.rs
```

## Components

### Lexer

- **Purpose**: Tokenizes the source code.
- **Directory**: `src/lexer`
- **Entry Point**: `src/lexer/main.rs`

### Parser

- **Purpose**: Converts tokens to an Abstract Syntax Tree (AST).
- **Directory**: `src/parser`
- **Entry Point**: `src/parser/main.rs`

### Semantic Analysis

- **Purpose**: Ensures the AST is semantically correct.
- **Directory**: `src/semantics`
- **Entry Point**: `src/semantics/main.rs`

### IR Generation

- **Purpose**: Transforms the AST to an Intermediate Representation (IR).
- **Directory**: `src/IR`
- **Entry Point**: `src/IR/main.rs`

### Optimization

- **Purpose**: Optimizes the IR.
- **Directory**: `src/optimizer`
- **Entry Point**: `src/optimizer/main.rs`

### Code Generation

- **Purpose**: Converts the optimized IR to Cairo Assembly (CASM).
- **Directory**: `src/codegen`
- **Entry Point**: `src/codegen/main.rs`

### `main.rs`

- **Purpose**: Overall entry point for the compiler.
- **Directory**: Root of `src/`
- **Entry Point**: `src/main.rs`

### `mod.rs`

- **Purpose**: Module declarations and possibly shared definitions.
- **Directory**: Root of `src/`
- **File**: `src/mod.rs`