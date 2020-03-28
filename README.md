# Hello Page

This is a personal "hello" page for [bradyjoslin.com](https://bradyjoslin.com) built with [Svelte](https://svelte.dev). It lives at [https://github.com/bradyjoslin/hello](https://github.com/bradyjoslin/hello).

Inspired by [janbaudisch/zola-hallo](https://github.com/janbaudisch/zola-hallo).

## Get started

Install the dependencies...

```bash
npm install
```

...then start [Rollup](https://rollupjs.org):

```bash
npm run dev
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running. Edit a component file in `src`, save it, and reload the page to see your changes.

## Building and running in production mode

To create an optimised version of the app:

```bash
npm run build
```

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies`.

## Deploying to Cloudflare Workers

To preview:

```bash
wrangler preview --watch
```

To publish:

Push to the master branch of this repo which will trigger a Github Action to publish using [Wrangler Action](https://github.com/cloudflare/wrangler-action).
