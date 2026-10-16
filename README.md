# Shortform Kit MCP server

Free remote MCP server for AI assistants (Claude, ChatGPT, Cursor, VS Code, Claude Code). No API key, no account.

**URL:** `https://shortformkit.com/mcp` (Streamable HTTP)

[![MCP status](https://shortformkit.com/api/mcp-badge?url=https%3A%2F%2Fshortformkit.com%2Fmcp)](https://shortformkit.com/mcp-server-tester/?url=https%3A%2F%2Fshortformkit.com%2Fmcp) [![Install in Cursor](https://cursor.com/deeplink/mcp-install-dark.svg)](https://cursor.com/en/install-mcp?name=shortformkit&config=eyJ1cmwiOiAiaHR0cHM6Ly9zaG9ydGZvcm1raXQuY29tL21jcCJ9) [![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_MCP-0098FF?logo=visualstudiocode&logoColor=white)](https://insiders.vscode.dev/redirect/mcp/install?name=shortformkit&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A//shortformkit.com/mcp%22%7D)

Platform guides with example prompts: [Instagram MCP server](https://shortformkit.com/instagram-mcp-server/), [TikTok MCP server](https://shortformkit.com/tiktok-mcp-server/), [YouTube MCP server](https://shortformkit.com/youtube-mcp-server/).

## Tools

| Tool | What it does |
|---|---|
| `get_video_info` | Title, author, duration, qualities, caption and hashtags of a public Instagram, YouTube, TikTok, X, Facebook or Pinterest post |
| `download_media` | MP4, MP3, image, cover or a frame at a timestamp, optionally only a section; returns a link valid for 15 minutes |
| `transcribe_video` | Whisper transcript with timestamps, 90+ languages, optional translation to English |
| `youtube_channel_id` | UC channel ID, handle, channel URL and RSS feed from a @handle or any video link |
| `social_video_specs` | 2026 upload specs (sizes, lengths, caption and hashtag limits) for 9 platforms, sourced |
| `creator_monetization` | Monetization programs and requirements, RPM by niche and country, engagement benchmarks, sponsorship rates |
| `loudness_and_subtitles` | LUFS and true peak targets (Spotify, YouTube, Netflix, EBU R128 …), subtitle rules, frame rates |
| `youtube_thumbnail_trends` | This week's measured thumbnail trends of the most-viewed new YouTube videos in 10 niches |
| `estimate_youtube_earnings` | Ad earnings range from monthly views and niche, or for Shorts |

## Add it

**Claude Code**

```
claude mcp add --transport http shortformkit https://shortformkit.com/mcp
```

**Cursor** (`~/.cursor/mcp.json`)

```json
{ "mcpServers": { "shortformkit": { "url": "https://shortformkit.com/mcp" } } }
```

**VS Code** (`.vscode/mcp.json`)

```json
{ "servers": { "shortformkit": { "type": "http", "url": "https://shortformkit.com/mcp" } } }
```

**Claude (claude.ai, desktop):** Settings, Connectors, Add custom connector, paste `https://shortformkit.com/mcp` (custom connectors depend on your plan).

## Notes

- Same fair-use rate limit per IP as the website. Downloads are deleted after 15 minutes.
- Only use it for content you own or are allowed to use.
- Data tools answer with sourced data (CC BY 4.0) from https://shortformkit.com/data/ and include the source URL.
- HTTP API description: https://shortformkit.com/openapi.json
- Guide: https://shortformkit.com/mcp-server/

## License

This repository (docs and registry metadata): MIT. Made by Diego Brügger, video editor in Zürich, for [Shortform Kit](https://shortformkit.com).
