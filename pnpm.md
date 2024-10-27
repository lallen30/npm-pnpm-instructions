# pnpm

## Install a Specific Version of `pnpm`

# Use `npm` to install `pnpm` globally with a specified version

npm install -g pnpm@9.4.0

## Manage pnpm Versions with corepack

# Enable corepack

corepack enable

# Install a specific version of pnpm

corepack prepare pnpm@9.4.0 --activate

# Verify the installation

pnpm -v

# Install a specific version of npm

pnpm env use 18.17.0

# Set the Installed Version as Default

export PNPM_HOME="$HOME/.local/share/pnpm"
export PATH="$PNPM_HOME:$PATH"

# switch to the new version of npm

pnpm env use 16.14.0
