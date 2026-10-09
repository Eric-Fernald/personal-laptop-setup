## Personal Laptop Setup
My personal setup and configuration files for a new software development laptop.

My main machine runs Windows 11 with WSL2 (Ubuntu 24.04). The `Brewfile` installs the same toolchain on macOS.

## Contents
- `install-vscode-extensions-windows.bat`: installs my VS Code extensions on Windows.
- `install-vscode-extensions-mac-linux.sh`: installs the same extensions on macOS or Linux.
- `Brewfile`: Homebrew packages, apps, and VS Code extensions for macOS.
- `settings.json`: my VS Code user settings.
- `.gitconfig`: my global Git configuration.
- `.gitignore_global`: global Git ignore rules, loaded through `core.excludesFile`.

There is no single install script. Run each step below that applies to the machine.

## VS Code Extensions Installation
The two scripts install the same list of extensions, grouped by these categories in the `Brewfile`:

- Python (Pylance, Ruff, Black, isort, Pylint, debugpy)
- Notebooks (Jupyter)
- Go
- .NET & C#
- C/C++ (C/C++ tools, Makefile Tools)
- Kotlin
- Web & JS (ESLint, Prettier, Vitest, Live Server)
- Cloud & IaC (Terraform, AWS Toolkit, Azure, Kubernetes)
- Containers (Docker, Docker Compose)
- Remote Dev (SSH, WSL, Dev Containers)
- AI Coding Agents (Claude Code, opencode)
- Git & GitHub (Git Graph, Git Blame, GitHub Pull Requests, GitHub Actions, GitStudio, Speedy Git)
- Data & Databases (PostgreSQL client, SQLite Viewer, Rainbow CSV, YAML)
- Code Quality (SonarLint, Error Lens, Debug Visualizer, Version Lens)
- Editor & Productivity (PowerShell, CodeSnap, vscode-pdf)
- Themes & UI (Material Icon Theme, Catppuccin icons, Cyberpunk 2077, Peacock)

To install on Mac/Linux:
```bash
chmod +x install-vscode-extensions-mac-linux.sh
./install-vscode-extensions-mac-linux.sh
```

To install on Windows:
```cmd
install-vscode-extensions-windows.bat
```

## Homebrew Package Installation
The `Brewfile` is for macOS. `brew bundle` installs the packages, apps, and VS Code extensions it lists.

1. Install Homebrew:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. From this directory, install everything in the Brewfile:
```bash
brew bundle
```

The Brewfile includes:
- Core tools: git, node, go, vim, zsh
- Python toolchain: python, pyenv, uv, poetry
- Dependencies: openssl@3, coreutils, wget, curl
- Cloud and container tools: awscli, kubernetes-cli, and terraform from the `hashicorp/tap` tap (homebrew-core's terraform is stuck at 1.5.7)
- Apps: VS Code, Docker Desktop, GitKraken, Obsidian, Google Chrome, iTerm2, .NET SDK, LM Studio, FileZilla, Discord
- Media: VLC, OBS
- The VS Code extensions listed above

## Git Configuration
`.gitconfig` sets my name and email, `main` as the default branch, VS Code as the editor, and `~/.gitignore_global` as the global ignore file.

To install on macOS/Linux:
```bash
ln -sf "$PWD/.gitconfig" ~/.gitconfig
ln -sf "$PWD/.gitignore_global" ~/.gitignore_global
```

To install on Windows:
```cmd
copy .gitconfig %USERPROFILE%\.gitconfig
copy .gitignore_global %USERPROFILE%\.gitignore_global
```

`core.autocrlf` and `credential.helper` use Windows values. On macOS or Linux, change `autocrlf` to `input` and the credential helper to `osxkeychain` (macOS) or `libsecret` (Linux). The comments in `.gitconfig` list these options.

## VS Code Settings
Copy `settings.json` to the VS Code user settings folder. This replaces any settings already there, so back up the existing file first if you want to keep it.

Windows:
```cmd
copy settings.json "%APPDATA%\Code\User\settings.json"
```

macOS:
```bash
cp settings.json ~/Library/Application\ Support/Code/User/settings.json
```

Linux:
```bash
cp settings.json ~/.config/Code/User/settings.json
```
