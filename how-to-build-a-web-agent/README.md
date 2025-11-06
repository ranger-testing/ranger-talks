# Building a Web Agent: Claude + Playwright MCP

First, clone this repo using your git client of choice.

Then, [install Claude Code](https://docs.anthropic.com/en/docs/claude-code/setup) if you don't already have it.

[Playwright MCP](https://github.com/microsoft/playwright-mcp) is an [MCP toolset](https://modelcontextprotocol.io/docs/getting-started/intro) that gives Claude the ability to control a browser and understand webpages.

Make sure your working directory is the git repo, and Configure Claude to use Playwright MCP:

```bash
cd ranger-talks
claude mcp add playwright npx -- @playwright/mcp@latest
```

Then run Claude and get logged in:

```bash
claude
```

Give Claude this instruction:

```markdown
You are working within how-to-build-a-web-agent/.
Read prompt.md.
Then read input.yaml, and follow the instructions in the prompt.
```

Note that if this is your first time ever running Playwright, Claude may need to install browsers before it can begin. This is normal - it needs specific builds of browsers that it can control.

## Gotcha!

There are at least two situations that may arise during this flow that challenge Claude. Historically these problems have been very difficult for a web agent:

- A marketing modal appears on the homepage a second or two after the initial page load
- There is persistent session storage, preventing Claude from proceeding to the next employee

Pay close attention, and see if Claude can work it out!

It may solve problems like this in a different way each time you run it...
