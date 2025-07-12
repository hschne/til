---
title: Claude Code Hooks 
date: 2025-07-12
tags: ai
---

# Claude Code Hooks 

Claude provides hooks to run after or before execution. This can be used to show notifications after execution finishes, for example. 

```json
# In ~/.claude/settings.json
"hooks": {
  "Notification": [
    {
      "matcher": "",
      "hooks": [
        {
          "type": "command",
          "command": "notify-send 'Claude Code' 'Finished working on your request or waiting for input'"
        }
      ]
    }
  ]
}
```

Source: [anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
