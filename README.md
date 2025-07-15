# youtube-transcript-mcp

A simple [MCP](https://modelcontextprotocol.io/) server that lets LLMs easily get the transcript of YouTube videos.

## To install

Add this to your LLM app's MCP settings:

```json
{
  "mcpServers": {
    "youtube-transcript": {
      "command": "bunx",
      "args": ["-y", "youtube-transcript-mcp"]
    }
  }
}
```

If you prefer node to bun, you can use `npx` instead:

```json
{
  "mcpServers": {
    "youtube-transcript": {
      "command": "npx",
      "args": ["youtube-transcript-mcp"]
    }
  }
}

