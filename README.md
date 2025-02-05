# Discord Time Display Activity

A simple Discord activity that displays the current time in a voice channel.

## Features
- Real-time clock display
- Discord activity integration
- Beautiful Discord-themed UI
- Debug logging

## Setup Instructions

1. Add the bot to your server using this link:
   [Bot Invite URL](https://discord.com/oauth2/authorize?client_id=1336526920464072847&permissions=8&scope=bot%20applications.commands)

2. Configure the Activity in Discord Developer Portal:
   - Go to [Discord Developer Portal](https://discord.com/developers/applications/1336526920464072847/activities)
   - Set "Activity Type" to "Embedded App"
   - Add URL Mapping:
     - ROOT MAPPING: `/`
     - TARGET: `https://YOUR_USERNAME.github.io/discord-time-activity`
   - Enable "Activity Launcher"

3. Run the Discord bot:
   ```bash
   python test.py
   ```

## Usage
- Type `!activity` in any channel to start the time display in your current voice channel
- Type `!activity <channel_id>` to start it in a specific voice channel
- Use `/activity` slash command for the same functionality

## Development
This project consists of two parts:
1. A static web interface (hosted on GitHub Pages) that displays the time
2. A Discord bot that creates activity invites

The web interface is hosted at `https://YOUR_USERNAME.github.io/discord-time-activity` and uses the Discord Embedded App SDK to integrate with Discord's activity system. 