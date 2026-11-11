# EasyEnv MCP

Connect your AI assistant to [EasyEnv](https://easyenv.io): create interviews,
build labs and challenges, and manage your workspaces without leaving the chat.

> **Status: in development.** The hosted server at `https://mcp.easyenv.io/mcp`
> is not live yet. This repository will hold the install instructions and the
> Claude Code plugin once it is.

There is nothing to install and no token to copy. Every client uses the same
hosted server: you click **Connect**, sign in to EasyEnv as you normally do,
approve access, and you are back in the chat.

## Server URL

```
https://mcp.easyenv.io/mcp
```

## Claude (claude.ai and Claude Desktop)

Settings → Connectors → **Add custom connector**, paste the URL above, then
**Connect** and sign in to EasyEnv.

## ChatGPT

Settings → Apps & Connectors → **Create**, paste the URL above, choose OAuth,
then sign in to EasyEnv.

## Claude Code

```
/plugin marketplace add donedeploy/easyenv-mcp
/plugin install easyenv@easyenv
```

Or add the server directly:

```sh
claude mcp add --transport http easyenv https://mcp.easyenv.io/mcp
```

Run `/mcp` inside Claude Code to sign in.

## Other MCP clients

Any client that supports remote MCP servers over Streamable HTTP with OAuth
(Cursor, VS Code, Windsurf and others) can use the same URL.

## Accounts

One EasyEnv sign-in covers every account you belong to. Tools that change
something take the account explicitly, so the assistant never writes to the
wrong one.

## Privacy

Interview results are not available through the assistant unless you turn
that on yourself in EasyEnv.

## Support

hello@easyenv.io
