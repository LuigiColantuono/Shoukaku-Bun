## Shoukaku-Bun

<p align="center"><a href="https://github.com/sponsors/LuigiColantuono"><img src="https://img.shields.io/github/sponsors/LuigiColantuono?style=social"></a> <a href="https://paypal.me/l0g4n7"><img src="https://img.shields.io/badge/💖-Support-ff69b4"></a> <img src="https://img.shields.io/npm/v/shoukaku-bun"> <img src="https://img.shields.io/npm/dm/shoukaku-bun?label=downloads"> <img src="https://img.shields.io/npm/l/shoukaku-bun"> <img src="https://img.shields.io/github/repo-size/LuigiColantuono/Shoukaku-Bun"> <a href="https://github.com/LuigiColantuono/Shoukaku-Bun"><img src="https://img.shields.io/badge/Bun-Networking-black?logo=bun"></a></p>

> Powerful, Lightweight wrapper around Lavalink

<p align="center">
    <img src="https://azurlane.netojuu.com/images/thumb/d/dc/ShoukakuWeddingWithoutBG.png/767px-ShoukakuWeddingWithoutBG.png" width="400"> 
</p>

### Features

- **Bun-Native**: Re-engineered to run exclusively on Bun.Purged all Node.js legacy dependencies (like `ws`).
- **Zero Latency**: Uses Bun's kernel-level WebSocket for maximum throughput.
- **Ultra Lightweight**: Optimized for minimal memory footprint (production tested at ~33MB).
- **TypeScript Native**: No build step required. Direct execution from source.
- **Stable & Updated**: Based on the rock-solid Shoukaku v4.2.0 logic.
- **Very cute (Very Important)**

## 📦 Bundle Size Comparison

| Package | Size | Dependencies | Total Install |
|---------|------|--------------|---------------|
| shoukaku | 366 kB | ws (~300 kB) | **~666 kB** |
| shoukaku-bun | 72.9 kB | **NONE** | **72.9 kB** |

**89% smaller install size!** 

## 🎵 The Story

Built out of frustration with constant WebSocket upgrade warnings that were 
making my Discord music bot laggy. After migrating to Bun, I realized the 
entire Shoukaku stack could be rewritten to be faster and lighter.

**Result?** Zero warnings. Noticeably faster. Way more fun to work with.

If this solved your problems too, [consider supporting the project](https://paypal.me/l0g4n7)! 
Even a coffee helps keep the motivation high! ☕

### Installation

```bash
bun add shoukaku-bun
```

### Official Documentation

> https://guide.shoukaku.shipgirl.moe/
> https://github.com/shipgirlproject/Shoukaku

## Performance
<img width="380" height="" src="https://i.imgur.com/zZsPzm6.png" />

## Support
> Kazagumo support server: https://discord.gg/nPPW2Gzqg2 (anywhere lmao)   
> Shoukaku support server: https://discord.gg/FVqbtGu (#development)           
> Brucius support server: https://discord.gg/XqJw52d35R

