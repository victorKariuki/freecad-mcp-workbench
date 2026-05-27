# Robust MCP Bridge Workbench

> [!IMPORTANT]
> **DISCLAIMER:** This is **NOT** the official release of this workbench.
> This repository is a mirrored copy based on the official [v0.6.2 release](https://github.com/spkane/freecad-addon-robust-mcp-server/releases/tag/robust-mcp-workbench-v0.6.2) by [@spkane](https://github.com/spkane).
>
> It exists solely to facilitate installation via the FreeCAD Addon Manager (**Preferences > Addon > Custom Repositories**) in cases where the official addon is unavailable or hard to locate. For the official project and documentation, please visit [spkane/freecad-robust-mcp-and-more](https://github.com/spkane/freecad-robust-mcp-and-more).

**Version:** 0.6.3

## Installation

### Via FreeCAD Addon Manager (Custom Repository)

The repository is fully ready for the FreeCAD Addon Manager:
**URL:** [https://github.com/victorKariuki/freecad-mcp-workbench](https://github.com/victorKariuki/freecad-mcp-workbench)

To use it in FreeCAD:
1. Go to **Tools > Addon Manager**.
2. Click the **Preferences** (gear icon) in the bottom right.
3. Go to the **Workbenches** or **Custom Repositories** tab.
4. Add the URL above: `https://github.com/victorKariuki/freecad-mcp-workbench`
5. Search for "**Robust MCP Bridge**" in the main Addon Manager list.

### Manual Installation

Copy the contents of this archive to your FreeCAD Mod directory:

- **macOS**: `~/Library/Application Support/FreeCAD/Mod/FreecadRobustMCPBridge/`
- **Linux**: `~/.local/share/FreeCAD/Mod/FreecadRobustMCPBridge/`
- **Windows**: `%APPDATA%/FreeCAD/Mod/FreecadRobustMCPBridge/`

## Usage

1. Switch to the **Robust MCP Bridge** workbench.
2. Click **Start MCP Bridge** in the toolbar.
3. Connect your MCP client (Claude Code, etc.).

## MCP Client Configuration

### Claude Code / Claude Desktop

Add the following to your `~/.claude/claude_desktop_config.json` (or a project-specific `.mcp.json` file):

```json
{
  "mcpServers": {
    "freecad": {
      "command": "freecad-mcp",
      "env": {
        "FREECAD_MODE": "xmlrpc"
      }
    }
  }
}
```

*Note: This configuration assumes the `freecad-mcp` command is installed and available in your system path.*

## Documentation

Full documentation: https://github.com/spkane/freecad-robust-mcp-and-more

## License

MIT License - see LICENSE file
