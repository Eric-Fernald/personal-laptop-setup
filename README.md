## dotfiles
My personal setup and configurations for deploying a new laptop for software development

## Installation
Run the `install.sh` script to set up your environment. This script will:
- Install Homebrew (if not already installed)
- Install Zsh and set it as the default shell   
- Install Oh My Zsh for managing Zsh configurations
- Install VSCode and set up my preferred extensions
- Install Git and set up my preferred configurations
- Install Node.js and npm
- Install Python and pip

## VS Code Extensions Installation

This repository includes scripts to install a curated set of VS Code extensions for both Windows and Mac/Linux:

- Windows: Run `install-vscode-extensions-windows.bat`
- Mac/Linux: Run `install-vscode-extensions-mac-linux.sh` 

The scripts will install extensions for:

- Python development (Pylance, debugpy, Jupyter support)
- Cloud development (AWS Toolkit, Docker, Kubernetes)
- AI/ML tools (GitHub Copilot, Claude)
- Remote development (SSH, WSL, Containers)
- Git integration (GitLens, Git Graph)
- Language support (Python, C++, C#, Kotlin)
- Productivity tools (CodeSnap, Rainbow CSV, Error Lens)
- Themes and icons (Material Icon Theme, Cyberpunk 2077)

To install on Mac/Linux:
```bash
chmod +x install-vscode-extensions-mac-linux.sh
./install-vscode-extensions-mac-linux.sh
```

To install on Windows, simply run the .bat file:
```cmd
install-vscode-extensions-windows.bat
```

## Homebrew Package Installation

This repository includes a `Brewfile` that automates the installation of necessary development tools and applications on macOS.

To use the Brewfile:

1. Install Homebrew if you haven't already:
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Install everything in the Brewfile:
```bash
brew bundle
```

The Brewfile includes:
- Core development tools (git, node, python, vim, zsh)
- Cloud and container tools (docker, kubernetes, terraform, aws-cli)
- Common development dependencies (openssl, coreutils, wget)
- GUI applications (VS Code, iTerm2, Docker Desktop)
- All VS Code extensions listed above

**Note:** Some VS Code extensions might need additional configuration after installation, particularly those requiring authentication like GitHub Copilot.