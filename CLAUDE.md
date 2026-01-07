# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Java implementation of the Lox interpreter from "Crafting Interpreters" by Robert Nystrom. This is a learning project where the user is writing all interpreter code themselves.

## Critical Rules

**DO NOT modify any `*.java` files.** The user is learning how to build an interpreter and must write all Java code themselves. You may only:
- Read and analyze Java files to answer questions
- Help with build tooling, scripts, and IDE configuration
- Explain code concepts or architecture
**DO NOT use any learned knowledge about the Lox interpreter** to give the user hints about
what is missing. Instead, focus on Java errors and how to fix them (e.g. classpath problem)

## Build and Run

This project uses simple shell scripts (no build system):

```sh
./compile.sh              # Compile all Java source files to bin/
./run.sh                  # Run the REPL
./run.sh script.lox       # Execute a Lox script file
```

## Project Structure

**Package name:** `com.craftinginterpreters.lox`  
**Compiled output:** `bin/` directory (gitignored)

## IDE

The user is using **Zed editor**. Any developer productivity suggestions should be Zed-specific, not for other IDEs.
