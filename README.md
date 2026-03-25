# githits-gemini-cli

Code examples from global open source for developers and AI assistants.

GitHits extension for [Gemini CLI](https://github.com/google-gemini/gemini-cli). Connects your assistant to the [GitHits](https://githits.com) MCP server for access to code examples from open source.

## Install

```sh
gemini extensions install https://github.com/githits-com/githits-gemini-cli
```

## Authentication

GitHits requires authentication. Gemini handles this automatically — on first use it will open your browser for OAuth authorization.

If you run into authentication issues, you can manage credentials manually:

```sh
npx githits login         # Log in via browser
npx githits auth status   # Check authentication status
npx githits logout        # Remove stored credentials
```

## Tools

Once installed, your Gemini assistant gets three tools:

| Tool | Purpose |
|---|---|
| `search` | Find code examples by describing what you need |
| `search_language` | Look up supported programming language names |
| `feedback` | Rate search results to improve future quality |

The assistant uses these tools automatically when it needs code examples.

## Requirements

- Node.js 20 or later
- [Gemini CLI](https://github.com/google-gemini/gemini-cli)

## License

MIT
