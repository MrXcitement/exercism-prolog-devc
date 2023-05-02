# Exercism Prolog

 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Overview
An [Exercism Prolog track](https://exercism.org/tracks/prolog) Devcontainer project. It defines a Devcontainer with the Exercism client and SWI Prolog v9.0.4 installed.

The project is designed to allows you to work through the Exercism Prolog track exercises using the Visual Studio Code editor and the Devcontainer running in a local Docker instance, a remote Docker instance or in a GitHub Codespaces environment.

The project expects that your Exercism files will be in a `prolog` subfolder.

## Requirements
It is expected:
- You have an Exercism account.

### Local development requires
- A Container Engine installed locally
  - Windows: Docker Desktop 2.0+ on Windows 10/11 Pro/Enterprise.
  - macOS: Docker Desktop 2.0+
  - Linux: Docker CE/EE 18.06+ and Docker Compose 1.21+.
- Git
- [Visual Studio Code](https://code.visualstudio.com/)
- Visual Studio Code [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) extensions are installed in VS Code.

### Remote development requires
- A Container Engine on your remote server
  - Linux: Docker CE/EE 18.06+ and Docker Compose 1.21+.
  - 2 GB RAM and a 2-core CPU is recommended.
- Git
- [Visual Studio Code](https://code.visualstudio.com/)
- Visual Studio Code [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) extensions are installed in VS Code.

### GitHub Codespaces requires
- No requirements, just open the Codespace remotely in a web browser.
- **Or** Install VS Code locally and install the [GitHub Codespaces](https://marketplace.visualstudio.com/items?itemName=GitHub.codespaces) extension. This will allow you to open the remote Codespace in a local VS Code instance.

## Usage
### Start a Local container
- Clone this repository from GitHub.
- Open the repository in Visual Studio Code.
- Reopen in Container. (`Dev Containers: Reopen in Container`)
### Start a Github Codespaces container
- Browse to this repository on GitHub.
- Click the `<> Code` button
- Click the `Codespaces` tab.
- Click the `+` to add a new Codespace using this repository
### Configure the Exercism cli
- Open a terminal inside the container. (`View: Toggle Terminal` <kbd>Ctrl</kbd>+<kbd>`</kbd>)
- Configure the exercism cli with your token and set the workspace folder to the root folder of this project.
  ```sh
  $ exercism configure -t <your token> -w "$PWD"
  ```
### Download the exercise
- Use the exercism cli to download the exercise to work on from the prolog track.
  ```sh
  $ exercism download -t prolog -e hello-world
  ```
- Edit the provided exercise file until the provided tests pass.
### Submit the exercise solution
- Submit your solved exercise.
  ```sh
  $ exercism submit hello_world.pl
  ```

## Related Sites
- [Exercism Prolog Track](https://exercism.org/tracks/prolog)
- [SWI Prolog](https://www.swi-prolog.org/)
- [Devcontainers](https://containers.dev/)
- [Visual Studio Code Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers)
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- [Docker Engine](https://docs.docker.com/engine/)
- [GitHub Codespaces](https://docs.github.com/en/codespaces)
