# LuckPermsLogger Plugin

LuckPermsLogger is a Minecraft plugin designed to log LuckPerms events and send these logs to a Discord channel using a bot. This plugin depends on the DiscordVelocityPlus plugin for its Discord integration.

## Features

- Sends LuckPerms logs to a specified Discord channel using a Discord bot.
- Configurable via in-game commands.
- Toggle logging on or off as needed.

## Commands

- `/lpl reload`  
  Reloads the plugin configuration.

- `/lpl set channel <channelId>`  
  Sets the Discord channel ID where logs will be sent.

- `/lpl set bot <botName>`  
  Sets the name of the Discord bot used for logging.

- `/lpl set toggle`  
  Toggles whether the bot will send logs to Discord or not.

## Dependencies

- [DiscordVelocityPlus]()  
  Ensure you have this plugin installed and configured correctly as LuckPermsLogger relies on it for Discord communication.

## Installation

1. Download the LuckPermsLogger plugin jar file.
2. Place the jar file in the `plugins` directory of your Minecraft server.
3. Ensure you have DiscordVelocityPlus installed and configured.
4. Start your server to generate the default configuration files for LuckPermsLogger.
5. Configure the plugin using the generated configuration files and the provided commands.

## Configuration

Below is an example configuration for LuckPermsLogger:

```yaml
enabled: false # Set to true to enable the feature

discord:
  bot_name: "bot_name" # The name of the bot as set in the Discord Velocity Plus configuration
  channel_id: 123 # The ID of the Discord channel