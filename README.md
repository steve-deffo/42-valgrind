# 42 Valgrind Container

A containerized environment for running Valgrind against C and C++ projects from the 42 curriculum.

## Purpose

Valgrind is not available natively on every development platform. This repository provides a reproducible environment for detecting memory leaks, invalid reads and writes, and file-descriptor issues without changing the host machine.

## Highlights

- Isolated Valgrind environment
- Reproducible memory checks
- Support for C and C++ binaries
- Practical debugging workflow for 42 projects

## Getting started

```bash
git clone https://github.com/steve-deffo/42-valgrind.git
cd 42-valgrind/42-ValgrindContainer
```

Follow the container configuration in the project directory to build the image, mount your source code, and run Valgrind against the compiled executable.

## Typical command

```bash
valgrind --leak-check=full --show-leak-kinds=all --track-fds=yes ./program
```

## Context

Built as a development utility while studying systems programming at [42 Abu Dhabi](https://42abudhabi.ae/).
