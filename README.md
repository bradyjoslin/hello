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

## Personalize content

Update the content using variables in App.svelte, for example:

```JavaScript
  let greeting = "Hello!";
  let identify = "I am Brady.";
  let image_url = "./static/images/portrait.jpg";
  let links = [
    { name: github, url: "https://github.com/bradyjoslin" },
    { name: twitter, url: "https://twitter.com/bradyj" },
    { name: linkedin, url: "https://linkedin.com/in/bradyjoslin" }
  ];
```

Bio information goes in My_Bio.svelte as HTML within the Bio component.

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

## Alternative Ways of Deploying to the Web

Other ways to deploy the app as [documented](https://github.com/sveltejs/template#deploying-to-the-web) in the Svelte Template.

### With [now](https://zeit.co/now)

Install `now` if you haven't already:

```bash
npm install -g now
```

Then, from within your project folder:

```bash
cd public
now deploy --name my-project
```

As an alternative, use the [Now desktop client](https://zeit.co/download) and simply drag the unzipped project folder to the taskbar icon.

### With [surge](https://surge.sh/)

Install `surge` if you haven't already:

```bash
npm install -g surge
```

Then, from within your project folder:

```bash
npm run build
surge public my-project.surge.sh
```
