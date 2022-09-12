# mcproto-rs
# Only Protocol Version 753 works

This is an implementation of serialization and deserialization of the minecraft protocol.

This crate can be used to implement any version of the minecraft protocol

To implement your own protocol, consult this example, and use the macros to define a protocol to your heart's content!

More documentation to come, just dumping the code since I finished it.

Usage:
```toml
[dependencies]
mcproto-rs = { git = "https://github.com/muno9748/mcproto-rs.git" }
```

## `#![no_std]`

You can use this crate without the standard library (but requiring `alloc`) by setting `default-features = false` in 
your Cargo.toml. This will only disable the `UUID4::random()` function, which requires `OsRandom` to generate a random UUID.
