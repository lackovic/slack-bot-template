# slack-bot-template

A Slack Bot template written in JavaScript/Node

## Prerequisites

- Node.js (version specified in `.nvmrc`)

- An account in a Slack workspace

## Setup

1. Create a new app or use existing one in [Slack API](https://api.slack.com/apps)

1. Open the app page

1. copy `.env.tpl` to `.env`

1. Enter your secrets in `.env`

1. _Slack app page_ > _Events subscription_ > _Enable events_

1. enter in `Request URL` the URL where you are running the bot + `/slack/events` (use [ngrok](https://ngrok.com/) to create URL to your localhost server through any NAT or firewall)

1. expand _Subscribe to bot events_ and add `message.im` event

1. _Slack app page_ > reinstall your app

1. press _Save Changes_

1. _Slack app page_ > _Interactivity & Shortcuts_ > enable _Interactivity_

1. enter in `Request URL` the same URL entered above

1. press _Save Changes_

## Running

```sh
npm start
```

## Using the bot

1. Open Slack

1. Select _Add apps_ from the left menu

1. Select the app you have created above

1. Type anything

1. Expect the bot to send you a greeting message

## References

- [Getting started with Bolt for JavaScript](https://slack.dev/bolt-js/tutorial/getting-started)
