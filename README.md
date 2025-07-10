
# MCP Build Chess Server

This is a fun MCP (Model Context Protocol) project that provides a simple server for interacting with the Chess.com public API. It demonstrates how to build and expose chess-related tools using the MCP framework.

## Features
- Query Chess.com player profiles and stats
- Exposes tools as MCP endpoints
- Easy to run and extend

## Project Structure

- `src/chess/chess_api.py`: Functions to call Chess.com public API
- `src/chess/server.py`: MCP server exposing chess tools
- `main.py`: Simple entry point
- `pyproject.toml`: Project configuration

## Installation

Install dependencies (MCP Server):

```bash
    "Chess": {
      "command": "uvx",
        "args": [
            "--from",
            "git+https://github.com/aruganga/MCP-CHESS.git",
            "chess"
        ]
    }
```

## Usage

You can run the MCP chess server with:

```bash
/Users/aruganga/.local/bin/uv --directory /Users/aruganga/Learning/mcp-ai-agent/mcp-build-chess-server run chess
```

Or, if installed as a package:

```bash
chess
```

## Example Tools

- `get_chess_player_profile(username: str)`: Get a Chess.com player's public profile
- `get_chess_player_stats(username: str)`: Get a Chess.com player's stats

## Fun & Extensible

This project is a playful demonstration of MCP and chess API integration. You can easily add more endpoints or connect to other chess APIs for more features!

---
Enjoy exploring chess data with MCP!