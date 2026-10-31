# WolfSMS for Cursor

Let AI agents securely read the text messages on your phone, like verification codes and OTPs.

This plugin connects Cursor to the hosted [WolfSMS](https://usewolfsms.com) MCP server at `https://usewolfsms.com/mcp`.

## Installation

### Cursor Marketplace

In Cursor, type `/add-plugin` in chat, search for **WolfSMS**, and install it.

### From source

Cursor loads local plugins from `~/.cursor/plugins/local/<plugin-name>/`:

```bash
git clone https://github.com/antislophq/wolfsms-mcp.git
mkdir -p ~/.cursor/plugins/local
rsync -a --delete --exclude='.git' wolfsms-mcp/ ~/.cursor/plugins/local/wolfsms/
```

Then run **Developer: Reload Window**.

## Usage

The first time the agent uses WolfSMS, Cursor asks you to sign in to WolfSMS. No API keys or configuration are needed.

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
- Email: support@usewolfsms.com
- Issues: [github.com/antislophq/wolfsms-mcp/issues](https://github.com/antislophq/wolfsms-mcp/issues)

## License

[MIT](./LICENSE)
