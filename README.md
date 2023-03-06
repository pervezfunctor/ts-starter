# Getting Started

### Install `pnpm`

Install pnpm by following the instructions on [pnpm install](https://pnpm.io/installation)

### Install `node`

Run the following command

```bash
pnpm env use --global latest
```

You need to install some npm packages globally:

```bash
pnpm install -g degit ndb @antfu/ni tsx turbo
```

### Install Editor

Install `visual studio code` with the following `winget` command:

```powershell
winget install --id Microsoft.VisualStudioCode
```

Alternatively, or even preferably use the instructions at [dotfiles](https://github.com/pervezfunctor/mini-dotfiles.git) to setup your Ubuntu/WSL environment. If you are on Windows 11, install WSL 2 first.

```powershell
  wsl --install -d Ubuntu
```

For more details refer to [wsl install](https://learn.microsoft.com/en-us/windows/wsl/install)

## Setup repository

Clone the repository:

```bash
degit pervezfunctor/ts-starter
cd ts-starter
```

Install dependencies:

```bash
pnpm install
```

## Common commands

To run app(development server):

```bash
pnpm dev
```

**Open [http://localhost:5173](http://localhost:5173)**

To run tests and watch for changes:

```bash
pnpm test:dev
```

To type check your code:

```bash
pnpm types:dev
```
