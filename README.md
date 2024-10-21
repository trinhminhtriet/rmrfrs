# 🧹 rmrfrs

🧹 rmrfrs is a powerful filesystem cleaning tool designed to optimize storage by identifying and removing unnecessary files within known project structures.

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

## ✨ Features

- **Recursive Search**: Scans directories and subdirectories for recognized project structures.
- **Space Savings**: Estimates the amount of space that can be freed by deleting redundant files.

## 🚀 Installation

To install **rmrfrs**, simply clone the repository and follow the instructions below:

```bash
git clone https://github.com/trinhminhtriet/rmrfrs.git
cd rmrfrs

cargo install --path .

rmrfrs --help
rmrfrs code/my_project code/my_project_2
rmrfrs --older 3M
rmrfrs -o3M
```

Running the below command will globally install the rmrfrs binary.

```bash
cargo install rmrfrs
```

Optionally, you can add `~/.cargo/bin` to your PATH if it's not already there

```bash
echo 'export PATH="$HOME/.cargo/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## 💡 Usage

Run **rmrfrs** with the following command to start cleaning your filesystem:

```sh
./rmrfrs [options] [path]
```

## 🤝 How to contribute

We welcome contributions!

- Fork this repository;
- Create a branch with your feature: `git checkout -b my-feature`;
- Commit your changes: `git commit -m "feat: my new feature"`;
- Push to your branch: `git push origin my-feature`.

Once your pull request has been merged, you can delete your branch.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
