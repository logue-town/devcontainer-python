# Python 3.13 Dev Container

A ready-to-use **Dev Container** for Python 3.13 development.

This project provides a pre-configured, reproducible development environment built on Docker. It's designed to get you started quickly with a clean Python 3.13 environment.

## Features

- 🐍 **Python 3.13**: The latest version of Python.
- 🧹 **Ruff**: Integrated as the default linter and code formatter for consistent, high-quality code.
- 🧰 **IDE Ready**: Pre-configured for both **VS Code** and **JetBrains IDEs** (like PyCharm). When you open this project, the Ruff extension/plugin will be installed automatically.
- 💾 **Format on Save**: Code is automatically formatted by Ruff whenever you save a Python file.

## Getting Started

To use this development environment, you need to have Docker and a supported IDE installed.

1.  **Clone this repository** to your local machine.
2.  **Open the project folder** in a supported IDE:
    -   **VS Code**: With the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension installed.
    -   **PyCharm** or other JetBrains IDEs with dev container support.
3.  When prompted, choose to **"Reopen in Container"**.

The IDE will build the Docker image defined in `.devcontainer/Dockerfile` and start the dev container. Your development environment with Python 3.13 and Ruff will be ready to use.

## Configuration

The dev container is configured through the following files:

-   `.devcontainer/devcontainer.json`: Defines the container's settings, including which IDE extensions to install and the UI settings for enabling Ruff.
-   `.devcontainer/Dockerfile`: The recipe for building the Docker image. It starts from a base Python 3.13 image and installs Ruff.

You can customize the environment further by editing these files. For example, you can add more Python packages to the `Dockerfile` or install more extensions in `devcontainer.json`.
