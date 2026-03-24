# githits-gemini-cli

Code examples from global open source for developers and AI assistants.

GitHits extension for [Gemini CLI](https://github.com/google-gemini/gemini-cli). Connects your assistant to the [GitHits](https://githits.com) MCP server for access to code examples from open source.

## Install

```sh
gemini extensions install https://github.com/githits-com/githits-gemini-cli
```

## Authentication

GitHits requires authentication. Two options:

### Browser Login (recommended)

```sh
npx githits login
```

Opens your browser for secure OAuth authentication. Tokens are stored locally and refreshed automatically.

### API Token

For environments where browser login is not practical, set an API token. Gemini CLI will prompt you to enter the token securely on first use, or you can set it manually:

```sh
export GITHITS_API_TOKEN=ghi-your-token-here
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
