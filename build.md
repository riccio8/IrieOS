# For compiling

## Linux
```bash
cargo rustc -- -C link-arg=-nostartfiles
```

## Windows
```bash
cargo rustc -- -C link-args="/ENTRY:_start /SUBSYSTEM:console"
```

## macOS
```bash
cargo rustc -- -C link-args="-e __start -static -nostartfiles"
```

### Install x86_64 target
```bash
rustup target add x86_64-unknown-none
```
## Compile using the .json file
```bash
cargo build --target .\x86_64-IrieOS.json
```
