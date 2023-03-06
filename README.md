# Getting Started

If you are on Windows 11, you must install WSL 2 which is nothing but Ubuntu on Windows.


## Setup System

### Install `pnpm`

Install pnpm by following the instructions on [pnpm install](https://pnpm.io/installation)

If you already have `node` installed, but don't have `pnpm` installed, you can run:

```bash
npm install -g pnpm npm
```

### Install `node`

If you don't have node, Install `node` using `pnpm`:

```bash
pnpm env use --global latest
```

You need to install some npm packages globally:

```bash
pnpm install -g degit ndb @antfu/ni tsx turbo
```


Install `visual studio code` with the following `winget` command:

```powershell
winget install --id Microsoft.VisualStudioCode
```

Alternatively, even preferrably use the following guide to setup your system.


### Install WSL 2 on Windows 11

```powershell
  wsl --install -d Ubuntu
```

For more details refer to [wsl install](https://learn.microsoft.com/en-us/windows/wsl/install)

### Install everything on Ubuntu/WSL

Follow instructions at [dotfiles](https://github.com/pervezfunctor/mini-dotfiles.git)

## Setup repository

Clone the repository:

```bash
git clone https://github.com/pervezfunctor/ts-starter.git
```

Install all the packages every time you run `git pull` including first time you clone this repository:

```bash
pnpm install
```

## Common commands

To run development server:

```bash
pnpm dev
```

To run tests and watch for changes:

```bash
pnpm test:dev
```

Open the terminal inside `Visual Studio Code`, and run the following command to
continuously watch for type errors:

```bash
pnpm types:dev
```

**Open [http://localhost:5173](http://localhost:5173) with your browser to see
the result.**
