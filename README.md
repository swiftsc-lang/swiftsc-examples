# SwiftSC Examples

A collection of example smart contracts demonstrating the features of SwiftSC V1.0.2-beta.

## 📦 Categories

### 🛠️ Module System (`examples/modules`)
Demonstrates how to organize your project into multiple files using `use` and `pub`.
- `math.stc`: A basic library module.
- `main.stc`: The main contract that imports from `math`.

**To build**:
```bash
swiftsc build examples/modules/main.stc --root examples/modules -o main.wasm
```

### ⚠️ Error Handling (`examples/error_handling`)
Demonstrates the `Result<T, E>` type and the `?` operator for clean error propagation.
- `error_test.stc`: A simple banking example showing balanced checks.

**To build**:
```bash
swiftsc build examples/error_handling/error_test.stc -o error.wasm
```

### 📚 Other Examples
- `hashmap_test.stc`: Usage of the storage-aware `HashMap`.
- `arc_test.stc`: Automatic Reference Counting and memory management.
- `syntax-showcase.stc`: A comprehensive look at the SwiftSC syntax.

## 🚀 Running Examples

You can run these examples in the local simulator:
```bash
swiftsc simulate examples/modules/main.stc --func test
```
