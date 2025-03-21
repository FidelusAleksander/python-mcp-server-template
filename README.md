# Python MCP Server Template

[![Python 3.13+](https://img.shields.io/badge/python-3.13+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A minimal template for creating a [Model Context Protocol (MCP)](https://github.com/modelcontextprotocol) server using the [Python SDK](https://github.com/modelcontextprotocol/python-sdk).


## :wrench: Setup

> [!TIP]
> If you want to create your own server, [create a new repository using this template.](https://github.com/new?template_owner=FidelusAleksander&template_name=python-mcp-server-template&owner=%40me&name=python-mcp-server)

### :package: Prerequisites

- [uv](https://docs.astral.sh/uv/) for package management
- Python 3.13+ (`uv python install 3.13`)

### :gear: Setup Python environment

Install all dependencies and activate the virtual environment

```bash
uv sync
source .venv/bin/activate
```

## :rocket: How to use

The server can be run in multiple ways:

### :robot: Visual Studio Code

The configuration to run this server in VSCode is already included in [`.vscode/mcp.json`](./.vscode/mcp.json).

All you need to do is Open VS Code Copilot Edits (Agent Mode)

> [!NOTE]
> At the time of writing this, MCP is only available in [Visual Studio Code Insiders version](https://code.visualstudio.com/insiders/)

### :microscope: Development Mode

The fastest way to test and debug your server is with the [MCP Inspector](https://github.com/modelcontextprotocol/inspector):

```bash
mcp dev server/main.py
```

or you can run your server directly

```bash
python server/main.py
```

## :books: Documentation

For more information about the Model Context Protocol:
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk)
- [Model Context Protocol Specification](https://github.com/modelcontextprotocol/mcp)

## :page_with_curl: License

This project is licensed under the [MIT License](LICENSE)

