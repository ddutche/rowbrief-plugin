# Rowbrief for Claude

Rowbrief is one project plan that a person, the people they work with, and each of
their AIs read and write. This plugin connects Claude to it and teaches Claude how to work
from it: read the plan, take the briefing for a task its person claimed for it, record
what it finds with honest confidence and links to the work, finish or block the task, and
propose changes for a person to approve.

## What is in it

- **A connector** (`.mcp.json`): the Rowbrief server at
  `https://rowbrief.inkcroft.com/mcp`. Connecting asks you to sign in to Rowbrief
  and approve Claude for the projects you tick, choosing what it may do there.
- **One skill** (`skills/working-from-the-shared-plan/SKILL.md`): how to use the server's
  tools well, in plain words.

## What it runs, sends and fetches

Nothing runs on your computer. The plugin holds no code, only the connector's address and
the skill's text. When Claude uses a tool, it sends that tool's request to the Rowbrief
server above, signed in as you, and only for the project you approved: reading the plan, or
recording an update, a status or a proposal on it. The server never reads your chats,
your files or Claude's memory.

## How to use it

1. Have a Rowbrief account and a project: https://rowbrief.inkcroft.com
2. Install the plugin, and connect the Rowbrief connector when Claude asks.
3. On the website, claim a task and pick Claude as its tool.
4. Ask Claude: "Show me the project."

Full documentation, including every tool and what stays with people:
https://rowbrief.inkcroft.com/docs

## Privacy

What Rowbrief keeps, who handles it and how to have it deleted:
https://rowbrief.inkcroft.com/privacy

Terms: https://rowbrief.inkcroft.com/terms

## Support

support@inkcroft.com
