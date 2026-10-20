<img src="media/logo.png" alt="ULO Logo" width="400px">

#

# Dev Env - MacOS                                               

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

# Installation for MacOS

Let\'s start by checking if you already have the necessary components.

```zsh
# Run in zsh / bash

git --version \
node --version \
php --version \
composer --help \
docker --version

```

If any of the commands do not exist follow the instructions to install
them.

## Homebrew

As an alternative to the individual instructions bellow, we can use a
package manager like Homebrew (<https://brew.sh/>) to install these
components. The benefit is that we can manage (install, remove, update)
all from one tool.
```zsh

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"


# Search for a package / Install a package

brew search \<package\>\
brew install \<package\>\
\
\# Update packages

brew upgrade
```

## Git

Download the installer from the official website,
<https://git-scm.com/downloads/mac>, and run it. The default options
presented by the install wizard are OK for our purposes.\
In addition we can consider any of these (or other) GUI options:

- Github Desktop: <https://desktop.github.com/download/>

- GitKraken Desktop: <https://www.gitkraken.com/>

## Node

For MacOS we have the option of having a CLI version manager for Node,
we can follow the instructions from the official website,
https://nodejs.org/en/download , detailed bellow.

```zsh
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.8/install.sh | bash

# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"

# Download and install Node.js:
nvm install 24

# Verify the Node.js version:
node -v # Should print "v24.22.0".

# Verify npm version:
npm -v # Should print "11.19.1".
```


In addition, we can consider other CLI tools that help with performance
/ resource management, like:

- YARN: <https://yarnpkg.com/>

- PNPN: <https://pnpm.io/>

- Bun: <https://bun.com/>

## PHP / Composer / Laravel

In a shell run this command. It installs PHP, Composer and the Laravel
CLI:

```zsh
/bin/bash -c "$(curl -fsSL https://php.new/install/mac/8.5)"
```

In addition, we can consider using a GUI tool like Laravel Herd,
<https://herd.laravel.com/> . This tool allows us to graphically manage
Laravel projects. The only downside is that it only manages Laravel, so
the rest of our toolset needs different management workflows.

## Code Editor

The recommend code editor for our project is Visual Studio Code. We can
install it from the official website,
<https://code.visualstudio.com/download>.

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

Download the installer from the official website,
<https://docs.docker.com/desktop/setup/install/mac-install/> , and run
the installer with the default options.
