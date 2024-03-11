## Prerequisites

```
cargo install probe-rs --locked --features cli
rustup target add thumbv7em-none-eabihf
```

## Programmer/debugger hardware

https://github.com/rp-rs/rp2040-project-template/blob/main/debug_probes.md#raspberry-pi-pico

## Run/Debug 

Connect the probe, then `cargo run`.

To see `defmt` messages, compile with the `DEFMT_LOG` environment variable
set appropriately. (By default, `defmt` will show only error level messages.)

Powershell (Windows)
```
$Env:DEFMT_LOG="trace"
```

Bash (Linux/macOS)
```
export DEFMT_LOG=trace
```
