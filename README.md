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

To install just copy the generated library file to your libraries directory:

```sh
cp build/thread.so ~/.config/lite-xl/libraries/
```

You can also install the Lua plugins to take advantage of the threads:

```sh
cp plugins/projectsearch.lua ~/.config/lite-xl/plugins/
cp plugins/findfileimproved.lua ~/.config/lite-xl/plugins/
```

## Api Docs

You can view the API documention on the [docs](docs/thread.lua) subdirectory.

## Plugins using threads for better performance:

* [projectsearch.lua](plugins/projectsearch.lua) -
  customized project search with multi threaded support for faster searching
  in the magnitude of 5-10x better performance.
* [findfileimproved.lua](plugins/findfileimproved.lua) -
  overrides default lite-xl find file functionality and adds threading support
  to scan a project files making it faster to search for files on big source trees.
