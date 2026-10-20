<img src="media/logo.png" alt="ULO Logo" width="400px">

#

# Dev Env - Linux                                               

## Objective

This worksheet will help you install all the necessary tools for the
Distributed Application Development course. We\'ll be building
applications using Laravel (API), Vue.js (Frontend), and Socket.IO
(Real-time communication), other tech stacks and and should be explored
but this is out of scope for this worksheet.

Required Tools

You will need to install the following tools:

- Git -- version control system.

- Node.js (v20 of higher) -- JavaScript runtime for frontend and
  real-time services.

- PHP (v8.4 or higher) -- Backend language for Laravel

- Composer -- PHP Dependency manager

- Code Editor -- VS Code recommended

- Docker -- Container solution for deployment

# Installation for Linux

Let\'s start by checking if you already have the necessary components.

```bash
# Run in zsh / bash

git --version \
node --version \
php --version \
composer --help \
docker --version

```

If any of the commands do not exist follow the instructions to install
them.

## Package Manager

Depending on our Linux Distribution there will be a package manager to
help install some of these packages, we just need to be aware that if we
are using a "stable" distro some of the language packages (PHP, node)
might not be the latest versions.

## Git

Git should be available on most distros, if not its safe to install from
the package manager.\
In addition we can consider any of these (or other) GUI options:

- Github Desktop: <https://desktop.github.com/download/>

- GitKraken Desktop: <https://www.gitkraken.com/>

## Node

For MacOS we have the option of having a CLI version manager for Node,
we can follow the instructions from the official website,
https://nodejs.org/en/download , detailed bellow.

```bash
# Download and install fnm:

curl -o- https://fnm.vercel.app/install \| bash

# Download and install Node.js:

fnm install 22

# Verify the Node.js version:

node -v # Should print \"v22.20.0\".

# Verify npm version:

npm -v # Should print \"10.9.3\".
```

In addition, we can consider other CLI tools that help with performance
/ resource management, like:

- YARN: <https://yarnpkg.com/>

- PNPN: <https://pnpm.io/>

- Bun: <https://bun.com/>

## PHP / Composer / Laravel

In an shell run this command. It installs PHP, Composer and the Laravel
CLI:
```bash
/bin/bash -c "$(curl -fsSL https://php.new/install/linux/8.5)"
```
## Code Editor

The recommend code editor for our project is Visual Studio Code. We can
install it from the distros' package manager.

The advantage of using a tool like VSCode is its ecosystem, the
following are recommended extensions that will help with our development
efforts:

- Laravel:
  <https://marketplace.visualstudio.com/items?itemName=laravel.vscode-laravel>

- Vue (Official):
  <https://marketplace.visualstudio.com/items?itemName=Vue.volar>

- PHP Intelephense:
  <https://marketplace.visualstudio.com/items?itemName=bmewburn.vscode-intelephense-client>

- ESLint:
  <https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint>

- Prettier:
  <https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode>

In addition, we can look at other IDEs like:

- JetBrains PHP Storm: <https://www.jetbrains.com/phpstorm/>

- JetBrains Web Storm: <https://www.jetbrains.com/webstorm/>

We can access JetBrains products for education here:
<https://www.jetbrains.com/academy/student-pack/>

## Docker

Install using the package manager following the instructions from the
official website, <https://docs.docker.com/engine/install/>.
