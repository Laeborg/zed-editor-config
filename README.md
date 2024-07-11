# Zed Editor
My personal configuration for [Zed Editor](https://github.com/zed-industries/zed).  
Running on Windows 11 with WSL2.

## Installation
For installation on Windows you currently need to build from source manually:
1. Install Rust on a x86_64 Microsoft Windows: https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe
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
5. Run the zed.exe from `target/release/` directory from within the cloned repository. I suggest to right-click and select `Send to > Desktop (create shortcut)` and then move this shortcut into `C:\ProgramData\Microsoft\Windows\Start Menu\Programs` for easy access through the Windows Start Menu.

## Configuration
After installation open the App Data directory: `C:\Users\<UserName>\AppData\Roaming\Zed` and clone this repository using Git:
```
git clone https://github.com/Laeborg/zed-editor-config .
```

This will configure `themes`, `keymap` and `settings` as defined in this repository.

## Extensions
Extensions are stored in `C:\Users\<UserName>\AppData\Local\Zed\extensions`.  
Installation is handled manually through the Extensions module.  

| Extension Name | Version | Repository |
| -------------- | ------- | ---------- |
| Dockerfile     | 0.0.4   | https://github.com/d1y/dockerfile.zed |
| HTML           | 0.1.1   | https://github.com/zed-industries/zed/tree/main/extensions/html |
| SQL            | 1.0.0   | https://github.com/evrensen467/zed-sql |
| PHP            | 0.0.6   | https://github.com/zed-industries/zed/tree/main/extensions/php |
| LOG            | 0.0.3   | https://github.com/evrensen467/zed-log |
