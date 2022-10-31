### <div align="center">Reservoir Discord Bot</div>
<div align="center">An open source Discord bot built using Reservoir</div>

## About The Project
Reservoir Discord Bot provides communities easy to use commands and alerts for their 
Discord server, which can be expanded and customized to their liking.

The Discord bot ships with the following functionality:
- Automated alerts for new floor listings and top collection bids
- Collection search to view stats and the current top bid

## Getting Started
### Prerequisites
1. Install [Node.js and NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
2. Install [Redis](https://redis.io/docs/getting-started/installation/)
3. Request a free [Reservoir API Key](https://docs.reservoir.tools/reference/overview#/0.%20Auth/postApikeys)
4. [Setup a Discord application and bot](https://discordjs.guide/preparations/setting-up-a-bot-application.html#setting-up-a-bot-application)

### Built With
- [ReservoirKit Client](https://docs.reservoir.tools/docs/reservoirkit-client)
- [Reservoir Protocol and API](https://reservoir.tools/)
- [TypeScript](https://www.typescriptlang.org/)
- [Discord.js](https://discord.js.org/#/)

### Installation
Fork this repo and follow these instructions to install dependencies.

```
$ npm install
```

### Configuration
Environment Variables
| Environment Variable | Required | Description                                                                                                                                           | Example                                                     |
|----------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|
| TOKEN                | `true`   | [Your Discord bot's token](https://discordjs.guide/preparations/setting-up-a-bot-application.html#your-bot-s-token)                                   | NzkyNzE1NDU0MTk2MDg4ODQy.X-hvzA.Ovy4MCQywSkoMRRclStW4xAYK7I |
| APPLICATION_ID       | `true`   | [Your Discord application id](https://support-dev.discord.com/hc/en-us/articles/360028717192-Where-can-I-find-my-Application-Team-Server-ID-)         | 5736050287834562                                            |
| CHANNEL_ID           | `true`   | [The Discord channel you want the bot active in](https://support.discord.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-) | 123456789098765432                                          |
| TRACKED_CONTRACT     | `true`   | The contract address of the collection you want to be alerted of floor price and top bid changes                                                      | 0xb47e3cd837ddf8e4c57f05d70ab865de6e193bbb                  |
| RESERVOIR_API_KEY    | `true`   | Reservoir API key provided by the Reservoir Protocol. [Get your own API key](https://api.reservoir.tools/#/0.%20Auth/postApikeys).                    | 123e4567-e89b-12d3-a456-426614174000                        |

Optional Variables
| Constant | Required | Description                                                                                                                                           | Default |
|----------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
| ALERT_COOLDOWN              | `false`  | Number of seconds to wait before sending a new floor price or top bid alert                                   | 60s |
| PRICE_CHANGE_OVERRIDE      | `false`   | Percentage change in floor price to override alert cooldown         | 0.1 (10%) |

### Run the App
Once you have your setup ready, run:
```
$ npm run start
```

## Contact

Twitter: [@reservoir0x](https://twitter.com/reservoir0x)
Discord: [Reservoir Protocol](https://discord.gg/j5K9fESNwh)
Project Link: [Reservoir Protocol](https://reservoirprotocol.github.io/)
