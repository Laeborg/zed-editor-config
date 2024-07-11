# Zed Editor
My personal configuration for [Zed editor](https://github.com/zed-industries/zed).  
Running on Windows 11 with WSL2.

## Installation
For installation on Windows you currently need to build from source manually:
1. Install Rust on 64 bit Windows: https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe
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
5. Run the zed.exe from `target/release/` directory from within the cloned repository. I sugest to right click and select `Send to > Desktop (create shortcut)` and then move this shortcut into `C:\ProgramData\Microsoft\Windows\Start Menu\Programs` for easy access through the Windows Start Menu.

## Configuration
After installation open the App Data directory: `C:\Users\<UserName>\AppData\Roaming\Zed` and clone this repository using Git:
```
git clone https://github.com/Laeborg/zed-editor-config .
```

This will configure `themes`, `keymaps` and `settings` as defined here.

## Extensions
