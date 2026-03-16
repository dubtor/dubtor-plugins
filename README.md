# dubtor-plugins

Plugin marketplace for [Claude Code](https://claude.ai/code) by [@dubtor](https://github.com/dubtor).

## Available Plugins

| Plugin | Description |
|---|---|
| [fal-image](https://github.com/dubtor/fal-image-plugin) | AI image generation via fal.ai (Nano Banana 2) |

## Installation

```bash
# Add the marketplace
/plugin marketplace add dubtor/dubtor-plugins

# Install a plugin
/plugin install fal-image@dubtor-plugins
```

## Adding a New Plugin

1. Create the plugin in its own GitHub repo (see [Claude Code plugin docs](https://code.claude.com/docs/en/plugins))
2. Add an entry to `.claude-plugin/marketplace.json`:

```json
{
  "name": "your-plugin-name",
  "source": {
    "source": "github",
    "repo": "dubtor/your-plugin-repo"
  },
  "description": "Brief description",
  "version": "1.0.0",
  "keywords": ["relevant", "tags"],
  "category": "creative"
}
```

3. Commit and push — users pick up new plugins with `/plugin marketplace update`

## License

MIT
