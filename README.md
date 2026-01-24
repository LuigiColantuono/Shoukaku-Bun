## Shoukaku-Bun

> Powerfull, Lightweight wrapper around Lavalink

[![Discord]([https://img.shields.io/discord/423116740810244097?style=flat-square)]
[![npm](https://img.shields.io/npm/v/shoukaku-bun?style=flat-square)](https://www.npmjs.com/package/shoukaku-bun)
![Github Stars](https://img.shields.io/github/stars/LuigiColantuono/Shoukaku-Bun?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues-raw/LuigiColantuono/Shoukaku-Bun?style=flat-square)
![NPM](https://img.shields.io/npm/l/shoukaku-bun?style=flat-square)

<p align="center">
    <img src="https://azurlane.netojuu.com/images/thumb/d/dc/ShoukakuWeddingWithoutBG.png/767px-ShoukakuWeddingWithoutBG.png"> 
</p>

### Features

- **Bun-Native**: Re-engineered to run exclusively on Bun.Purged all Node.js legacy dependencies (like `ws`).
- **Zero Latency**: Uses Bun's kernel-level WebSocket for maximum throughput.
- **Ultra Lightweight**: Optimized for minimal memory footprint (production tested at ~33MB).
- **TypeScript Native**: No build step required. Direct execution from source.
- **Stable & Updated**: Based on the rock-solid Shoukaku v4.2.0 logic.
- **Very cute (Very Important)**

## 🎵 The Story

Built out of frustration with constant WebSocket upgrade warnings that were 
making my Discord music bot laggy. After migrating to Bun, I realized the 
entire Shoukaku stack could be rewritten to be faster and lighter.

**Result?** Zero warnings. Noticeably faster. Way more fun to work with.

If this solved your problems too, [consider supporting the project](https://paypal.me/tuonome)! 
Even a coffee helps keep the motivation high! ☕

### Installation

This is a specialized fork. Install it directly from GitHub:

```bash
bun add shoukaku-bun
```

### Documentation

> https://guide.shoukaku.shipgirl.moe/

### Getting Started

> https://guide.shoukaku.shipgirl.moe/guides/1-getting-started/

### Supported Libraries

> https://guide.shoukaku.shipgirl.moe/guides/5-connectors/

### Example Bot

> https://github.com/Deivu/Kongou

### Configuration Options

```js
// Parameters for main class init, Options is the Configuration Options
new Shoukaku(new Connectors.DiscordJS(client), Nodes, Options);
```

| Option                 | Type                   | Default  | Description                                                                                      | Notes                    |
| ---------------------- | ---------------------- | -------- | ------------------------------------------------------------------------------------------------ | ------------------------ |
| resume                 | boolean                | false    | If you want to enable resuming when your connection to lavalink disconnects |                          |
| resumeTimeout          | number                 | 30       | Timeout before lavalink destroys the players on a disconnect                                     | In seconds               |
| resumeByLibrary        | boolean                | false    | If you want to force resume players no matter what even if it's not resumable by lavalink        |                          |
| reconnectTries         | number                 | 3        | Number of tries to reconnect to lavalink before disconnecting                                    |                          |
| reconnectInterval      | number                 | 5        | Timeout between reconnects                                                                       | In seconds               |
| restTimeout            | number                 | 60       | Maximum amount of time to wait for rest lavalink api requests                                    | In seconds               |
| moveOnDisconnect       | boolean                | false    | Whether to move players to a different lavalink node when a node disconnects                     |                          |
| userAgent              | string                 | (auto)   | Changes the user-agent used for lavalink requests                                                | Not recommeded to change |
| structures             | Object{rest?, player?} | {}       | Custom structures for shoukaku to use                                                            |                          |
| voiceConnectionTimeout | number                 | 15       | Maximum amount of time to wait for a join voice channel command                                  | In seconds               |
| nodeResolver           | function               | function | Custom node resolver if you want to have your own method of getting the ideal node               |                          |

### Wrappers

| Name     | Link                                          | Description                                              |
| -------- | --------------------------------------------- | -------------------------------------------------------- |
| Kazagumo | [Github](https://github.com/Takiyo0/Kazagumo) | A wrapper for Shoukaku that has an internal queue system |

> Open a pr if you want to add a wrapper here

### Other Links

- [Discord](https://discord.gg/XqJw52d35R)

- [Lavalink](https://github.com/lavalink-devs/Lavalink)

### Code made with ❤ by @ichimakase (Saya) & Luigi

