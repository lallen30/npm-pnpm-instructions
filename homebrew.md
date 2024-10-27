# Homebrew

https://brew.sh

## Install Homebrew

# Run the following command to install Homebrew

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

## Install `nvm` with Homebrew

brew install nvm

## Set Up `nvm` in Your Shell Profile

# 1. Create a directory for `nvm`

mkdir -p ~/.nvm

# 2. Add the following lines to your shell profile (e.g., `~/.zshrc`, `~/.bashrc`, or `~/.bash_profile`)

export NVM_DIR="$HOME/.nvm"
[ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh" # This loads nvm

# 3. Restart your shell or source your profile to load `nvm`

source ~/.zshrc # or ~/.bashrc or ~/.bash_profile depending on your shell

## Test `nvm` Installation

# Verify the installation by checking the `nvm` version

nvm --version

---

# NOTE:

# Docker is not a Node.js package manager.

# Please ensure it is already installed on your system.

# Follow official instructions at https://docs.docker.com/desktop/

# Docker images are provided officially at https://github.com/nodejs/docker-node/

# pulls the Node.js Docker image

docker pull node:20-alpine

# verifies the right Node.js version is in the environment

docker run node:20-alpine node -v # should print `v20.18.0`

# verifies the right npm version is in the environment

docker run node:20-alpine npm -v # should print `10.8.2`
