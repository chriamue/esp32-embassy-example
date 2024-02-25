# ESP32-embassy-example

This is an example of how to use the embassy library with an ESP32.

## Requirements

```bash
cargo install cargo-espflash
cargo install espup
espup install
. $HOME/export-esp.sh
```

On Mac, if openssl does not work:

```bash
OPENSSL_NO_VENDOR=1 cargo install espup
OPENSSL_NO_VENDOR=1 cargo install cargo-espflash
```


## Flashing

```bash
cargo espflash flash --release --monitor
```

```bash
cargo +esp run --no-default-features --features=esp32s3 --release --target xtensa-esp32s3-none-elf
```


## Thanks to

- [Embassy on ESP: Getting Started](https://dev.to/apollolabsbin/embassy-on-esp-getting-started-27fi)
- [embassy](https://embassy.dev/)
