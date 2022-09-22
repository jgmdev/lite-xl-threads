# Lite XL Threads Plugin

Lite XL plugin that adds the missing API for threading functionality.

## Building

You will need to have meson and a working build environment for your operating
system. Then, to build just execute the following commands:

```sh
meson setup build
meson compile -C build
```

## Installation

To install just copy the generated library file to your plugins directory:

```sh
cp build/thread.so ~/.config/lite-xl/plugins/
```

## Api Docs

You can view the API documention on the [docs](docs/thread.lua) subdirectory.
