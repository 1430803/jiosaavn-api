<div align=center>

![][ci] ![][views] ![][stars] ![][forks] ![][issues] ![][license] ![][code-size] ![][commit-activity]

# 🎵 Jio Saavn API

### A simple wrapper for the Jio Saavn API powered by Hono.js 🔥.

[**📚 Documentation**](https://docs-jiosaavn.netlify.app/) (in progress)

## ✨ Features

</div>

- 🚀 **Ultrafast** - Powered by [Hono.js](https://hono.dev).The router `RegExpRouter` is really fast.
- 🪶 **Lightweight** - Has has minimal dependencies.
- 🌍 **Multi-runtime** - Works on `Bun`, `Node.js`, `Vercel` or `Cloudflare Workers`. The same code runs on all platforms.
- 🔥 Download High Quality Songs, w/ lyrics for supported songs.
- 🎵 Get Songs, Albums, Playlists, Artists, Radio Stations, Podcasts Lyrics, Recommendations, and more.
- ❤️ Open Source

<div align=center>

## 🛠️ Building from source

</div>

- Clone the repository

```
git clone https://github.com/rajput-hemant/jiosaavn-api-ts
cd jiosaavn-api-ts
```

- Install dependencies

```
bun i || pnpm i || npm i || yarn
```

#### Bun

> **Warning**
> You need to have [Bun.js](https://bun.sh) installed on your machine to run the project with bun.

```
bun run dev || pnpm dev || npm run dev || yarn dev
```

#### Node.js

```
bun run dev:node || pnpm dev:node || npm run dev:node || yarn dev:node
```

#### Vercel Dev Server

```
bun run dev:vercel || pnpm dev:vercel || npm run dev:vercel || yarn dev:vercel
```

#### Cloudflare Workers

> **Warning**
> Make sure to remove Node API code from `src/index.ts#` & [`config.ts`](./src/lib/config.ts#L8) before deploying or running the project with Cloudflare Workers.

[src/index.ts](./src/index.ts)

```diff
...

-  port: +(process.env.PORT ?? 3000),
+ port: 3000, # update accordingly

...
```

[src/lib/config.ts](./src/lib/config.ts#L8)

```diff
...

-  enableRateLimit: process.env.ENABLE_RATE_LIMIT === "true" ?? false,
+  enableRateLimit: false, # update accordingly
...

```

```
bun run dev:vercel || pnpm dev:cf || npm run dev:cf || yarn dev:cf
```

<div align = center>

## 🌐 Deploying your own instance

You can easily deploy your own hosted version of the `JioSaavn API` by clicking on one of the links below, which will set up a ready-to-go version for you:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/sumitkolhe/jiosaavn-api)

[![Deploy with Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/rajput-hemant/jiosaavn-api-ts)

**OR**

#### Deploying using CLI

</div>

- Vercel (utilizes Edge Functions and can automatically execute in the region nearest to the user who triggers them.)
- It's worth noting that `Mumbai, India (South) - bom1` is the recommended region for this project deployment.

```
bun run deploy:vercel || pnpm deploy:vercel || npm run deploy:vercel || yarn deploy:vercel
```

- Cloudfare Workers

```
bun run deploy:cf || pnpm deploy:cf || npm run deploy:cf || yarn deploy:cf
```

<div align=center>

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🦾 Contributors:

<a href="https://github.com/rajput-hemant/jiosaavn-api-ts/graphs/contributors" target="blank"> <img src="https://contrib.rocks/image?repo=rajput-hemant/jiosaavn-api-ts&max=500" />

</div>

<!----------------------------------{ Labels }--------------------------------->

[views]: https://komarev.com/ghpvc/?username=jiosaavn-api-ts&label=view%20counter&color=red&style=flat
[code-size]: https://img.shields.io/github/languages/code-size/rajput-hemant/jiosaavn-api-ts
[issues]: https://img.shields.io/github/issues-raw/rajput-hemant/jiosaavn-api-ts
[license]: https://img.shields.io/github/license/rajput-hemant/jiosaavn-api-ts
[commit-activity]: https://img.shields.io/github/commit-activity/w/rajput-hemant/jiosaavn-api-ts
[forks]: https://img.shields.io/github/forks/rajput-hemant/jiosaavn-api-ts?style=flat
[stars]: https://img.shields.io/github/stars/rajput-hemant/jiosaavn-api-ts
[ci]: https://github.com/rajput-hemant/jiosaavn-api-ts/actions/workflows/ci.yml/badge.svg
