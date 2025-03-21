# Python MCP Server Template

[![Python 3.13+](https://img.shields.io/badge/python-3.13+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A minimal template for creating a [Model Context Protocol (MCP)](https://github.com/modelcontextprotocol) server using the [Python SDK](https://github.com/modelcontextprotocol/python-sdk).


## Setup

> [!TIP]
> If you want to create your own server, create a new repository using this template.

### Prerequisites

- [uv](https://docs.astral.sh/uv/) for package management
- Python 3.13+ (`uv python install 3.13`)

### Setup Python environment

Install all dependencies and activate the virtual environment

```bash
uv sync
source .venv/bin/activate
```

## Running the Server

The server can be run in multiple ways:

#### 1. Development Mode with the [MCP Inspector](https://github.com/modelcontextprotocol/inspector)

The fastest way to test and debug your server is with the MCP Inspector:

```bash
mcp dev server/main.py
```

#### 2. Direct Execution

Run the server directly with Python:

```bash
python server/main.py
```

## Documentation

For more information about the Model Context Protocol:
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk)
- [Model Context Protocol Specification](https://github.com/modelcontextprotocol/mcp)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

