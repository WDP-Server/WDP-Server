# AI Help System

**WDP-Help - AI-powered player assistance**

## Overview

AI assistant answers Minecraft questions using server context.

## Using AI Help

### Ask a Question

```
/help <your question>
```

**Examples:**
```
/help how do I get more SkillCoins?
/help what's the best armor?
/help how do I start the nether?
/help what quests should I do?
```

## Response Format

AI responses include:
- 📚 Context from server docs
- ⚡ Tool usage indicators
- Formatted Minecraft text

## Context System

AI knows about:
- Server rules and features
- Currency and shop
- Quest systems
- Skill progression
- Crafting recipes

### Relevance Scoring

| Score | Meaning |
|-------|---------|
| 10 | Server-specific |
| 7-9 | Server gameplay |
| 4-6 | General Minecraft |
| 1-3 | Off-topic |

## AI Configuration

### Model Options

| Model | Quality | Speed |
|-------|---------|-------|
| gpt-4o-mini | Good | Fast |
| gpt-4o | Better | Medium |
| claude-3-opus | Best | Slower |

### Settings

```yaml
ai:
  max-tokens: 1024
  temperature: 0.7
  timeout: 30
  stream: true
```

## History System

AI remembers 5 recent messages:
- Suggests help after 3 same questions
- Only saves relevant conversations

## Thinking Animation

While waiting:
```
● Thinking...
○ ● ○
○ ○ ●
```

## Troubleshooting

### AI Not Responding

- Check API key in config
- Verify internet connection
- Check rate limits

### Bad Responses

- Ask more specific questions
- Try different wording
- Check context files exist

## Commands

| Command | Description |
|---------|-------------|
| `/help <question>` | Ask AI |
| `/help stats` | View AI statistics |

## Tips

1. **Be specific** - "How do I get diamond?" not "Tell me about diamonds"
2. **Server questions** - AI knows your server
3. **Follow-up** - Ask clarifying questions
4. **Multi-part** - Complex questions step by step
