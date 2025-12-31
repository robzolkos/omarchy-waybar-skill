# Omarchy Waybar Skill

An agent skill for managing Waybar configuration using natural language.

## Overview

This skill enables AI coding agents to understand and modify your Waybar status bar configuration. It's designed for [Omarchy](https://omarchy.org/) Linux systems.

## Installation

### Claude Code

```bash
git clone https://github.com/robzolkos/omarchy-waybar-skill.git ~/.claude/skills/waybar
```

### OpenCode

```bash
git clone https://github.com/robzolkos/omarchy-waybar-skill.git ~/.config/opencode/skill/waybar
```

## Usage

Once installed, your agent will automatically use this skill when you ask about Waybar. Examples:

- "Add a memory monitor to my waybar"
- "Move the clock to the left side"
- "Remove the CPU indicator"
- "Add a custom module that shows disk usage"
- "Show battery percentage"
- "Make the bar thicker"
- "Hide the system tray"
- "Add a module that runs a script every 30 seconds"

## Features

- **Natural language configuration** - Describe what you want, the agent handles the JSON
- **Omarchy integration** - Uses Omarchy commands for reload/reset
- **Safe editing** - Automatic backups before changes, JSON validation after
- **Module management** - Add, remove, move, and configure modules
- **Custom modules** - Create new modules with exec scripts
- **Styling support** - Modify `style.css` for appearance changes

## Omarchy Commands

The skill uses these Omarchy commands:

| Command | Purpose |
|---------|---------|
| `omarchy-restart-waybar` | Restart Waybar |
| `omarchy-toggle-waybar` | Show/hide Waybar |
| `omarchy-refresh-waybar` | Reset to Omarchy defaults |

## Configuration Files

- `~/.config/waybar/config.jsonc` - Main configuration
- `~/.config/waybar/style.css` - Styling

## Requirements

- [Omarchy](https://omarchy.org/)
- Waybar

## License

MIT
