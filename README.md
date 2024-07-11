# Zed Editor
My personal configuration for [Zed editor](https://github.com/zed-industries/zed).  
Running on Windows 11 with WSL2.

## Installation
For installation on Windows you currently need to build from source manually:
1. Install from 64-bit Windows: https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.ex
2. Install the Rust WASM toolchain:
```
rustup target add wasm32-wasi
```
3. Clone down the [Zed editor](https://github.com/zed-industries/zed) repository on your locale machine:
```
git clone https://github.com/zed-industries/zed.git
```
4. Build the source code for release:
```
cargo run --release
```
5. Run the zed.exe from `target/release/` directory from within the cloned repository.

## Configuration


## Extensions
