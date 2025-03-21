# Python MCP Server Template

A minimal template for creating a Model Context Protocol (MCP) server using the [Python SDK](https://github.com/modelcontextprotocol/python-sdk).

## Overview

This template provides the basic structure for implementing an MCP server that can be used to serve AI models with context window management capabilities. The Model Context Protocol allows for efficient handling of context windows across multiple requests.

## Features

- Minimal MCP server implementation using FastMCP
- [uv](https://docs.astral.sh/uv/) for Python package management
- Sample tools, resources, and prompts
- Lifespan management with application context

## Getting Started

### Prerequisites

- Python 3.10+
- [uv](https://docs.astral.sh/uv/) for package management

### Installation

1. Create a new repository using this template
2. Clone your new repository
3. Install dependencies:

```bash
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
uv pip install -e .
```

### Running the Server

The server can be run in two ways:

#### Development Mode with the MCP Inspector

The fastest way to test and debug your server is with the MCP Inspector:

```bash
mcp dev src/server.py
```

#### Installing in Claude Desktop

Once your server is ready, install it in Claude Desktop:

```bash
mcp install src/server.py
```

#### Direct Execution

You can also run the server directly:

```bash
python main.py
# or
python src/server.py
```

## Customization

To customize the server for your specific model:

1. Modify the `AppContext` class in `src/server.py` to configure your model parameters
2. Add new tools by creating new functions decorated with `@mcp.tool()`
3. Add new resources by creating new functions decorated with `@mcp.resource()`
4. Add new prompts by creating new functions decorated with `@mcp.prompt()`

## Example Client

The `examples/client_example.py` file demonstrates how to interact with the MCP server as a client.

## Documentation

For more information about the Model Context Protocol:
- [MCP Python SDK](https://github.com/modelcontextprotocol/python-sdk)
- [Model Context Protocol Specification](https://github.com/modelcontextprotocol/mcp)

## License

MIT

