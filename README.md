[![Add to Cursor](https://fastmcp.me/badges/cursor_dark.svg)](https://fastmcp.me/MCP/Details/737/youtube-transcript)
[![Add to VS Code](https://fastmcp.me/badges/vscode_dark.svg)](https://fastmcp.me/MCP/Details/737/youtube-transcript)
[![Add to Claude](https://fastmcp.me/badges/claude_dark.svg)](https://fastmcp.me/MCP/Details/737/youtube-transcript)
[![Add to ChatGPT](https://fastmcp.me/badges/chatgpt_dark.svg)](https://fastmcp.me/MCP/Details/737/youtube-transcript)
[![Add to Codex](https://fastmcp.me/badges/codex_dark.svg)](https://fastmcp.me/MCP/Details/737/youtube-transcript)
[![Add to Gemini](https://fastmcp.me/badges/gemini_dark.svg)](https://fastmcp.me/MCP/Details/737/youtube-transcript)

# youtube-transcript-mcp

A simple [MCP](https://modelcontextprotocol.io/) server that lets LLMs easily get the transcript of YouTube videos.

## To install

Add this to your LLM app's MCP settings:

```json
{
  "mcpServers": {
    "youtube-transcript": {
      "command": "bunx",
      "args": ["--bun", "-y", "youtube-transcript-mcp"]
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
      "args": ["-y", "youtube-transcript-mcp"]
    }
  }
}
```

## To use

Just ask your LLM about a YouTube video:

> Summarize this video: https://www.youtube.com/watch?v=dQw4w9WgXcQ

> What are the three key points of this video? https://www.youtube.com/watch?v=dQw4w9WgXcQ

> What are some counterpoints to this argument here? https://www.youtube.com/watch?v=dQw4w9WgXcQ
