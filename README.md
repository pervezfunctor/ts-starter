# Getting Started

If you are on Windows 11, you must install WSL 2 which is nothing but Ubuntu on Windows.


## Install WSL 2 on Windows 11

```powershell
  wsl --install -d Ubuntu
```

For more details refer to [wsl install](https://learn.microsoft.com/en-us/windows/wsl/install)

Please Note: Following instructions will work on WSL 2 on Windows, Ubuntu or
macos. These won't work on Windows 11 terminal

## Setup repository

Clone the repository:

```bash
git clone https://github.com/pervezfunctor/ts-starter.git
```

If you don't have `node` installed, please run:

```bash
curl -fsSL https://get.pnpm.io/install.sh | sh -
pnpm env use --global latest
```

You need to install some npm packages globally:

```bash
pnpm install -g degit ndb @antfu/ni tsx turbo
```

If you do have `node` installed, but don't have `pnpm` installed, you must run:

```bash
npm install -g pnpm npm
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

## Contributing

Create a branch, like:

```bash
git checkout -b <your-branch>
```

Implement your feature or fix an issue. Commit your changes.

To send a pull request, rebase changes from the `main` branch. Then run the
following before doing `git push` to your branch and sending a pull request:

```bash
git checkout main
git pull
git checkout <your-branch>
git rebase main
pnpm install
pnpm ci
```
