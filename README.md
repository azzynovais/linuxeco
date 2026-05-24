# Linuxeco

Linuxeco is a curated development and creative ecosystem for Linux environments. It is designed to configure a standard installation into a functional workstation for developers and creative users. While it prioritizes open-source software, it includes necessary proprietary components to maintain standard functionality and parity with alternative UNIX operating systems such as macOS.

---

## Key Features

* **Automated Non-Interactive Deployment:** The script handles system updates, repository configuration, package acquisition, and dependency resolution without requiring manual input during execution.
* **Privilege Separation:** System utilities are installed via the root package manager, while user-specific tools, such as Homebrew, are sandboxed within the local user context.
* **Configuration Integrity:** The deployment process generates a timestamped backup copy of the existing configuration file before applying any modifications.

---

## Components Included

### Core Development Infrastructure
* **Build Systems and Toolchains:** `build-essential`, `gcc`, `g++`, `make`, `cmake`, `autoconf`, `automake`, `libtool`.
* **Version Control Management:** `git`, `git-lfs`, `subversion`.
* **Runtimes and Execution Environments:** Python 3 (`python3-venv`, `python3-dev`), Java (`default-jdk`), Node.js (via the official Nodesource LTS distribution channel), and Rust (via `rustup`).
* **User-Space Package Management:** Homebrew (Linuxbrew) configured for isolated user packages
