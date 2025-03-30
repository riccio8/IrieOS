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
