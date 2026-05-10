# Rux Compiler Tests

Sandbox for development and testing of the [Rux](https://github.com/rux-lang/Rux) compiler.

## Structure

```
Tests/
├── Pass/    # packages expected to compile and run successfully
└── Fails/   # packages expected to fail compilation
```

### Pass

| Test       | Description                          |
| ---------- | ------------------------------------ |
| Arithmetic | Basic arithmetic operations          |
| Assert     | Runtime assertions                   |
| Bool       | Boolean types and logic              |
| Calc       | Complex calculations                 |
| Enum       | Enumeration types                    |
| Fatal      | Fatal error handling                 |
| For        | For loops                            |
| Format     | String formatting                    |
| Functions  | Function definitions and overloading |
| If         | Conditional statements               |
| Import     | Package imports                      |
| Int        | Integer types                        |
| Interface  | Interface declarations               |
| Loop       | Loop constructs                      |
| Memory     | Memory management                    |
| Pointers   | Pointer types and operations         |
| Print      | Standard output                      |
| SizeOf     | Size-of operator                     |
| Slice      | Slice types                          |
| String     | String types and operations          |
| Struct     | Struct types                         |
| Tuple      | Tuple types                          |
| Union      | Union types                          |
| Var        | Variable declarations                |
| Variadic   | Variadic functions                   |
| While      | While loops                          |

### Fails

| Test  | Expected Error                             |
| ----- | ------------------------------------------ |
| Const | Reassignment of a constant                 |
| Empty | Package with no source files               |
| Let   | Reassignment of an immutable `let` binding |

## Usage

Build a package from its directory:

```sh
rux build
```

Run the compiled executable:

```sh
rux run
```

## License

[MIT](LICENSE)
