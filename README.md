# OpenClaw VPS Installation

OpenClaw AI personal assistant installed on VPS at 46.225.65.77

## What is OpenClaw?

OpenClaw is an open-source personal AI assistant that can:
- Chat via Discord, Slack, Telegram, WhatsApp, and more
- Execute code and commands
- Manage files and browse the web
- Remember context across conversations
- Run scheduled tasks (heartbeats)

**Version:** 2026.1.29

## Installation

This is an npm-based installation of OpenClaw.

```bash
cd /var/www/openclaw
npm install
```

## Running OpenClaw

### Start the Gateway (main server)
```bash
cd /var/www/openclaw
./node_modules/.bin/openclaw gateway --port 18789 --bind lan --verbose
```

### Run Onboarding Wizard
```bash
./node_modules/.bin/openclaw onboard
```

### Check Status
```bash
./node_modules/.bin/openclaw doctor
```

## Configuration

Config file location: `~/.openclaw/openclaw.json`

Workspace location: `~/.openclaw/workspace`

## Useful Commands

```bash
# Send a message
./node_modules/.bin/openclaw message send --to "+1234567890" --message "Hello"

# Open dashboard
./node_modules/.bin/openclaw dashboard

# Check logs
./node_modules/.bin/openclaw logs

# Memory search
./node_modules/.bin/openclaw memory search "topic"
```

## Links

- Website: https://openclaw.ai
- GitHub: https://github.com/openclaw/openclaw
- Docs: https://docs.openclaw.ai
