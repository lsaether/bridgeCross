# Welcome to bridgecross 👋

[![Version](https://img.shields.io/npm/v/bridgecross.svg)](https://www.npmjs.com/package/bridgecross)
[![Documentation](https://img.shields.io/badge/documentation-yes-brightgreen.svg)](https://github.com/daaniiieel/bridgecross#readme)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/daaniiieel/bridgecross/graphs/commit-activity)
[![License: GPL--3.0--or--later](https://img.shields.io/github/license/daaniiieel/bridgecross)](https://github.com/daaniiieel/bridgecross/blob/master/LICENSE)

> A simple, small and fast discord to telegram bridge written in node.js

## Install

```sh
npm install -g bridgecross
```

## Usage

- Create a Discord bot.
- Create a Telegram bot by talking to botFather
**IMPORTANT**: Make the bot an admin in your group, or go to BotFather -> bot settings and disable private mode.

- Create a Discord webhook. You can do this by going to Server settings -> Webhooks. Copy the URL, you'll need it later.

> If you want to run it on heroku, you can just click the button below.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/filcnaplo/bridgecross)

- Set env variables:

| Env variable                     | type   | value                                                                                                                                                                                         |
| -------------------------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `TELEGRAM_BOT_TOKEN`             | string | You can get this by speaking with @BotFather on telegram and creating a new bot.                                                                                                              |
| `DISCORD_TOKEN`                  | string | The bot token for your Discord application. Create a new app at the Discord Developer Portal , go to the bot section, click on Create a bot and copy the bot token it gives to you.           |
| `TELEGRAM_CHAT_ID`               | string | The ChatId of the telegram group you want to bridge.                                                                                                                                          |
| `DISCORD_CHANNEL_ID`             | string | The Discord ChannelId of the channel you want to bridge.                                                                                                                                      |
| `webhook_id` and `webhook_token` | string | Those are part of the webhook URL you copied. webhook_id is a 18 characters long int, webhook_token is a ~70 chars long randomly generated string. Those are seperated by slashes in the url. |

```sh
bridgecross
```
