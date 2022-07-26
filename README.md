# aries

Rust implementation of cycle-accurate NES emulator.

## Building and Running

### SDL2

Install the dependencies for Rust-SDL2( https://github.com/Rust-SDL2/rust-sdl2 ):

```sh
# Ubuntu
sudo apt install libsdl2-dev

# Arch Linux
sudo pacman -S sdl2

# MacOS
brew install sdl2
```

Build:

```
git clone --recursive https://github.com/tomoesaturn/aries.git
# git clone https://github.com/tomoesaturn/aries.git
# git submodule update --init --recursive

cargo build --workspace
```

Run:

```
cargo run --bin nes_sdl
```

### WASM

TODO

## Supported Mappers

- [x] Mapper000
- [ ] Mapper001

## Passed Tests

- [x] [Hello, World!](http://hp.vector.co.jp/authors/VA042397/nes/sample/helloworld.zip), from NES kennkyushitsu (Japanese) http://hp.vector.co.jp/authors/VA042397/nes/index.html
- [ ] nestest

## References and credits

- Referred C++ implementation: https://github.com/AndreaOrru/LaiNES
- Real-time rewindable emulator: https://github.com/ulfalizer/nesalizer
- Well documented Rust WASM implemantation: https://github.com/koute/pinky
- Circuit Diagram: https://console5.com/wiki/Nintendo_NES-001
- Circuit Diagram (Japanese): http://elec-junker-p2.blog.jp/FC_HVC-001%20HVC-CPU-05_REV07.pdf
- Nesdev Wiki: https://www.nesdev.org/wiki/Nesdev_Wiki
- Loopy's document for ppu scrolling: http://nesdev.org/loopyppu.zip
