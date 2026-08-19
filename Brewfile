# Brewfile - macOS half of my laptop setup.
# My daily driver is Windows 11 + WSL2 (Ubuntu 24.04); this file mirrors the
# same toolchain on macOS. Install everything with: brew bundle
#
# Note: homebrew/core, homebrew/cask, and homebrew/bundle are built into
# Homebrew 4.x and no longer need to be tapped.

# Taps
tap "hashicorp/tap"  # homebrew-core's terraform is frozen at 1.5.7 (BUSL relicense)

# Core Development Tools
brew "git"
brew "node"
brew "go"
brew "vim"
brew "zsh"

# Python Toolchain
brew "python"
brew "pyenv"     # pyenv-win on the Windows box
brew "uv"
brew "poetry"

# Development Dependencies
brew "openssl@3"
brew "coreutils"
brew "wget"
brew "curl"

# Cloud & Container Tools
brew "awscli"
brew "kubernetes-cli"
brew "hashicorp/tap/terraform"

# GUI Applications
cask "visual-studio-code"
cask "docker-desktop"
cask "gitkraken"
cask "obsidian"
cask "google-chrome"
cask "iterm2"
cask "dotnet-sdk"
cask "lm-studio"
cask "filezilla"
cask "discord"

# Media
cask "vlc"
cask "obs"

# VS Code Extensions
# Python
vscode "charliermarsh.ruff"
vscode "ms-python.black-formatter"
vscode "ms-python.debugpy"
vscode "ms-python.isort"
vscode "ms-python.pylint"
vscode "ms-python.python"
vscode "ms-python.vscode-pylance"
vscode "ms-python.vscode-python-envs"

# Notebooks
vscode "ms-toolsai.jupyter"
vscode "ms-toolsai.jupyter-keymap"
vscode "ms-toolsai.jupyter-renderers"
vscode "ms-toolsai.vscode-jupyter-cell-tags"
vscode "ms-toolsai.vscode-jupyter-slideshow"

# Go
vscode "golang.go"

# .NET & C#
vscode "ms-dotnettools.csharp"
vscode "ms-dotnettools.vscode-dotnet-runtime"

# C/C++
vscode "ms-vscode.cpp-devtools"
vscode "ms-vscode.cpptools"
vscode "ms-vscode.cpptools-extension-pack"
vscode "ms-vscode.cpptools-themes"
vscode "ms-vscode.makefile-tools"

# Kotlin
vscode "fwcd.kotlin"
vscode "mathiasfrohlich.kotlin"

# Web & JavaScript
vscode "dbaeumer.vscode-eslint"
vscode "esbenp.prettier-vscode"
vscode "vitest.explorer"
vscode "ms-vscode.live-server"
vscode "ritwickdey.liveserver"

# Cloud & Infrastructure as Code
vscode "4ops.terraform"
vscode "hashicorp.terraform"
vscode "ms-azuretools.vscode-azureterraform"
vscode "amazonwebservices.aws-toolkit-vscode"
vscode "ms-azuretools.vscode-azureresourcegroups"
vscode "ms-azuretools.vscode-azure-github-copilot"
vscode "ms-azuretools.vscode-azure-mcp-server"
vscode "ms-kubernetes-tools.vscode-kubernetes-tools"

# Containers
vscode "docker.docker"
vscode "ms-azuretools.vscode-docker"
vscode "ms-azuretools.vscode-containers"
vscode "formulahendry.docker-explorer"
vscode "p1c2u.docker-compose"

# Remote Development
vscode "ms-vscode-remote.remote-containers"
vscode "ms-vscode-remote.remote-ssh"
vscode "ms-vscode-remote.remote-ssh-edit"
vscode "ms-vscode-remote.remote-wsl"
vscode "ms-vscode-remote.vscode-remote-extensionpack"
vscode "ms-vscode.remote-explorer"
vscode "ms-vscode.remote-server"

# AI Coding Agents
vscode "anthropic.claude-code"
vscode "sst-dev.opencode"

# Git & GitHub
vscode "mhutchie.git-graph"
vscode "waderyan.gitblame"
vscode "github.vscode-pull-request-github"
vscode "github.vscode-github-actions"

# Data & Databases
vscode "cweijan.dbclient-jdbc"
vscode "cweijan.vscode-postgresql-client2"
vscode "qwtel.sqlite-viewer"
vscode "mechatroner.rainbow-csv"
vscode "phplasma.csv-to-table"
vscode "mohsen1.prettify-json"
vscode "redhat.vscode-yaml"

# Code Quality & Debugging
vscode "sonarsource.sonarlint-vscode"
vscode "usernamehw.errorlens"
vscode "hediet.debug-visualizer"
vscode "pflannery.vscode-versionlens"

# Editor & Productivity
vscode "ms-vscode.powershell"
vscode "ms-vscode.vscode-speech"
vscode "cardinal90.multi-cursor-case-preserve"
vscode "adpyke.codesnap"

# Themes & UI
vscode "pkief.material-icon-theme"
vscode "carlos18mz.cyberpunk-2077-rebuild"
vscode "johnpapa.vscode-peacock"
vscode "bierner.gif-player"
vscode "jakobhoeg.vscode-pokemon"
