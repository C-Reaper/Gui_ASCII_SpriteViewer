## Overview
The project is a C program that renders ASCII sprites using a custom library. It supports Linux, Windows, Wine, and WebAssembly builds.

## Features
- Render ASCII sprites from images.
- Supports loading and saving sprite files.
- Basic rendering functionality with position and color adjustments.

## Project Structure
### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools
- Libraries needed:
  - X11 for Linux (`libX11-dev`)
  - GDI32 for Windows
  - Wine for Wine build
  - SDL for WebAssembly

## Build & Run
### Build Process
To build the project, navigate to the project directory and use one of the following make commands:

- **Linux:**
  ```bash
  make -f Makefile.linux all
  ```
  
- **Windows:**
  ```bash
  make -f Makefile.windows all
  ```

- **Wine (Cross-compiling for Windows):**
  ```bash
  make -f Makefile.wine all
  ```

- **WebAssembly (Emscripten):**
  ```bash
  make -f Makefile.web all
  ```

### Execution
After building, you can run the executable using:

- **Linux:**
  ```bash
  make -f Makefile.linux exe
  ```

- **Windows:**
  ```bash
  make -f Makefile.windows exe
  ```

- **Wine (Cross-compiling for Windows):**
  ```bash
  make -f Makefile.wine exe
  ```

- **WebAssembly (Emscripten):**
  ```bash
  make -f Makefile.web exe
  ```

These commands will compile the source code, link it with necessary libraries, and produce an executable or HTML file depending on the target platform.