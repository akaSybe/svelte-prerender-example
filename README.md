# Prerender Svelte app at build-time

This is an example how to prerender Svelte app

## Get started

Install the dependencies

```bash
npm install
```

Build

```bash
npm run build
```

Run

```bash
npm run serve
```

Navigate to [localhost:5000](http://localhost:5000). You should see your app running

## How it works

Rollup config consists of two separate configs:

The first config used to build usual iife bundle with app.

The second config used to build root component as [SSR component](https://svelte.dev/docs#Server-side_component_API). When SSR component bundled, Rollup executes script `prerender.js`, which uses SSR Component API to get HTML and CSS.

## Remarks

It's experimental example. Maybe there is a more simple way.
