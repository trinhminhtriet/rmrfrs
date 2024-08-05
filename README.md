# rmrfrs 🧹

## rm -rf in Rust

Cleans `node_modules`, `target`, `build`, and friends from your projects.

Excellent if

- 💾 You want to back up your code but don't want to include GBs of dependencies
- 🧑‍🎨 You try out lots of projects but hate how much space they occupy
- ⚡️ You like keeping your disks lean and zippy

<br />

<p align="center">
    <strong>20+ Supported Project Types</strong>
</p>

<p align="center">
<a href="https://doc.rust-lang.org/cargo/">Cargo</a> (Rust),
<a href="https://cmake.org">CMake</a> (C, C++),
<a href="https://getcomposer.org/">Composer</a> (PHP),
<a href="https://elixir-lang.org/">Elixir</a>,
<a href="https://godotengine.org/">Godot 4.x</a> (C#, GDScript)
</p>
<p align="center">
<a href="https://gradle.com/">Gradle</a> (Java)
<a href="https://jupyter.org/">Jupyter Notebook</a> (Python),
<a href="https://pixi.sh/">Pixi</a> (Python),
<a href="https://maven.apache.org/">Maven</a> (Java),
<a href="https://nodejs.org/">Node</a> (JavaScript)
</p>
<p align="center">
<a href="https://dart.dev/">Pub</a> (Dart),
<a href="https://www.python.org/">Python</a>
<a href="https://www.scala-sbt.org/">SBT</a> (Scala),
<a href="https://docs.haskellstack.org/">Stack</a> (Haskell),
<a href="https://swift.org/">Swift</a>
</p>
<p align="center">
<a href="https://unity.com/">Unity</a> (C#),
<a href="https://www.unrealengine.com/">Unreal Engine</a> (C++),
<a href="https://ziglang.org/">Zig</a>,
<a href="https://dotnet.microsoft.com/">.NET</a> (C#, F#)
<a href="https://turbo.build/repo">Turborepo</a> (JavaScript)
</p>

**Source**

Requires [rust](https://www.rust-lang.org/tools/install). You may need [platform specific dependencies on linux](https://github.com/xi-editor/druid#platform-notes).

```sh
git clone https://github.com/trinhminhtriet/rmrfrs.git
cargo install --path rmrfrs/rmrfrs-ui
```

## Usage

> **Warning**
>
> `rmrfrs` is [_essentially_] `rm -rf` with a prompt. Use at your own discretion. Always have a backup of your projects.

### Command Line Interface

Running `rmrfrs` without a directory specified will run in the current directory.

```sh
rmrfrs
```

Supplying a path will tell `rmrfrs` where to start. Multiple paths are supported.

```sh
rmrfrs code/my_project code/my_project_2
```

Passing a time will filter projects to those that haven't been modified for at least the specified period. See `rmrfrs --help` for the full list of options.

```sh
rmrfrs --older 3M # only projects with last modified greater than 3 months
rmrfrs -o3M # shorthand
```

More options such as quiet mode, following symlinks, and filesystem restriction are viewable with `rmrfrs --help`.

## Building/Development

To build the cli `rmrfrs` you can run `cargo build` and `cargo run` from the projects root directory.

To build the gui `rmrfrs-ui` you must first navigate into the `rmrfrs-ui` directory, then you can run `cargo build` and `cargo run`.

The output binaries will be located in `target/debug/` or `target/release/` per [Cargo](https://doc.rust-lang.org/cargo/index.html) defaults.
