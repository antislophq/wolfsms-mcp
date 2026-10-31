# WolfSMS MCP

Securely access SMS messages on your phone, like delivery codes and transaction alerts.

This plugin connects your AI agent to the hosted [WolfSMS](https://usewolfsms.com) MCP server at `https://usewolfsms.com/mcp`. It follows the [Agent Plugins](https://agent-plugins.org) standard and also ships Cursor and Claude Code manifests.

## Installation

### Cursor

In Cursor, type `/add-plugin` in chat, search for **WolfSMS MCP**, and install it.

### Claude Code

```
/plugin marketplace add antislophq/wolfsms-mcp
/plugin install wolfsms@wolfsms
```

### Codex

```bash
codex plugin marketplace add antislophq/wolfsms-mcp
```

Then install **WolfSMS MCP** from the Plugins Directory.

### VS Code and GitHub Copilot

Run **Chat: Install Plugin From Source** from the Command Palette and enter `https://github.com/antislophq/wolfsms-mcp`.

### Any other MCP client

Add a remote MCP server with the URL `https://usewolfsms.com/mcp`.

## Usage

The first time the agent uses WolfSMS, your client asks you to sign in to WolfSMS. No API keys or configuration are needed.

Then ask the agent things like:

- "Link my phone to WolfSMS."
- "What's the verification code I just got?"
- "Show my latest text messages."

The agent walks you through installing the WolfSMS app and pairing your phone if it isn't linked yet.

## Tools

| Tool | Description |
| --- | --- |
| `link_phone` | Checks whether your phone is linked, and returns pairing instructions if it isn't. |
| `list_messages` | Lists SMS messages synced from your devices, newest first. |
| `list_devices` | Lists the devices that sync SMS messages. |

## Support

- Website: [usewolfsms.com](https://usewolfsms.com)
- Privacy: [usewolfsms.com/privacy](https://usewolfsms.com/privacy)
- Email: support@usewolfsms.com
- Issues: [github.com/antislophq/wolfsms-mcp/issues](https://github.com/antislophq/wolfsms-mcp/issues)

## License

[MIT](./LICENSE)
