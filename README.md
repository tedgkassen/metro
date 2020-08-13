## A library for parallel stream processing in Rust (in extremely early development. If you are here, this is not worth looking at)

Ex:
```rust
let out = Stream::from(v)
    .map(Box::new(|i| i + 1))
    .map(Box::new(|i| i.to_string()))
    .collect();

=> ["2", "3", "4", "5"]
```