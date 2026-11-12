# EasyEnv MCP

Connect your AI assistant to [EasyEnv](https://easyenv.io): create interviews,
build labs and challenges, and manage your workspaces without leaving the chat.

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

## What it can do

- **Labs:** list recipes and templates, plan a lab from a description, create, start, stop, extend and archive labs, save one as a template, invite people.
- **Tests and interviews:** browse templates and the question library, plan and create a test, add questions, invite candidates (sends real email, so the assistant asks you first).
- **Results:** list candidates, read and compare their results. Off until you turn it on in EasyEnv under Settings, Connected AI apps. Your own results as a candidate are always available.
- **Preparation:** roadmaps, courses, enrolment and progress, practice challenges and their results, practice positions.
- **Account:** your accounts, plan, credits and usage.

Deliberately not available: signup and payments, running commands on a machine, passwords and other secrets, and anything that would let a candidate answer a live interview through an assistant.

## Accounts

One EasyEnv sign-in covers every account you belong to. Tools that change
something take the account explicitly, so the assistant never writes to the
wrong one.

## Privacy

Interview results are not available through the assistant unless you turn
that on yourself in EasyEnv.

## Support

hello@easyenv.io
