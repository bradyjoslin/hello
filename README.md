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

You can run the newly built app with `npm run start`. This uses [sirv](https://github.com/lukeed/sirv), which is included in your package.json's `dependencies` so that the app will work when you deploy to platforms like [Heroku](https://heroku.com).

## Single-page app mode

By default, sirv will only respond to requests that match files in `public`. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

## Deploying to the Cloudflare Workers

To preview:

```bash
wrangler preview --watch
```

To publish:

```bash
wrangler publish
```

TODO: Setup GitHub action for deployment.
