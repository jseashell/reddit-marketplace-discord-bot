# Reddit Marketplace Discord Bot

A discord bot that monitors user-defined keywords on marketplace subreddits

## Table of Contents

- [Install](#install)
- [Link Reddit Account](#link-reddit-account)
- [Configure](#configure)
- [Run the App](#run-the-app)
- [Server Commands](#server-commands)
- [License](#license)

## Install

```sh
git clone git@github.com:jseashell/reddit-marketplace-discord-bot.git
cd reddit-marketplace-discord-bot
npm install
```

## Link Reddit Account

Create a Reddit script (app) through your Reddit account

1. Create an App in https://www.reddit.com/prefs/apps/
1. Select type `script`

> `redirect uri` does not matter but you have to fill it in with somethinga

**Take note of the App ID and Secret**

### Configure

1. Open `./config/config.json`
1. Paste the Reddit App ID into empty quotes for `reddit_app_id: "",`
1. Paste the Reddit App Secret into empty quotes for `reddit_app_secret: "",`
1. Open `./deals.json/` and set the shopping search keywords you're looking for {"keyword: "1080 ti"};

## Run the App

```sh
# Run the bot
npm start
```

## Server Commands

Command | Description | 
---  | ---
`!shop -r <subreddit>`| Shops a specific /r/ for the subscribed keywords in `deals.json` | 

 

## License

This software is distributed under the terms of the [MIT License](./LICENSE).
