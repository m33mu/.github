
![m33mu logo](https://raw.githubusercontent.com/m33mu/m33mu/main/png/m33mu.png)

# m33mu

**m33mu** is an embedded microcontroller emulator for ARMv8-M Cortex-M33.
It runs real firmware images - Secure, Non-secure, or both - directly on the
host, with no physical hardware.

It runs as an interactive terminal UI, a command-line emulator, and a tool
inside automated tests and CI jobs, with a built-in GDB remote server for
debugging.

This organization is home to the emulator and its accessory projects.

[![CI](https://github.com/m33mu/m33mu/actions/workflows/ctest.yml/badge.svg)](https://github.com/m33mu/m33mu/actions/workflows/ctest.yml)

[![Language](https://img.shields.io/badge/C-00599C?logo=c&logoColor=white)](https://github.com/m33mu/m33mu)

[![License](https://img.shields.io/badge/license-AGPLv3-green.svg)](https://github.com/m33mu/m33mu/blob/main/LICENSE)

## Repositories

| Repository | Description |
|---|---|
| [m33mu](https://github.com/m33mu/m33mu) | The emulator: Cortex-M33 core with TrustZone awareness, SoC profiles (STM32H5/U5/L5, LPC55S69, MCXW71C, MCXN947, i.MX RT700, RW612, nRF5340/54LM20, RP2350, PIC32CK, M2354), GDB server, TUI |

## Quick start

```sh
build/m33mu --cpu stm32h563 --uart-stdout --tui <firmware>.bin
```

See the [documentation](https://github.com/m33mu/m33mu#documentation-index)
for getting started, supported CPUs, and CI usage.

## License

Released under AGPLv3.
