# Idle Ring Game

A very barebones idle game made with raylib. The library is now included in this repository, so users don’t need to install it separately.

## Build instructions

### VS Code (all platforms)

Install a compiler toolchain for your platform before building; VS Code alone does not include one.

1. Open the project folder in VS Code.
2. Run the build task with **Ctrl+Shift+B** or **F5**

### Windows: MinGW-w64

From the project root, run:

```sh
make
```

Use a recent version of **MinGW-w64** rather than the older MinGW. You can get it from [w64devkit](https://github.com/skeeto/w64devkit/releases) or use the version installed with the raylib installer.

If you installed raylib with its installer, add `C:\raylib\w64devkit\bin` to your `PATH` so the compiler can be found. You do not need to install a second MinGW-w64 toolchain.

### Windows: Microsoft Visual Studio 2026

Build instructions for this toolchain are not documented yet.

### Linux

From the project root, run:

```sh
cd build
./premake5 gmake
cd ..
make
```

### macOS

From the project root, run:

```sh
cd build
./premake5.osx gmake
cd ..
make
```

<!--
add flag `--cc=clang` if using using clang?
`.\premake5 --cc=clang gmake`
-->

## Output

The built game is placed in `bin/`.
