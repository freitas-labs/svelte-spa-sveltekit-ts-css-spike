# create-svelte

Everything you need to build a Svelte project, powered by [`create-svelte`](https://github.com/sveltejs/kit/tree/master/packages/create-svelte).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

```bash
# create a new project in the current directory
npm create svelte@latest

# create a new project in my-app
npm create svelte@latest my-app
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
npm run dev

# or start the server and open the app in a new browser tab
npm run dev -- --open
```

## Building

To create a production version of your app:

```bash
npm run build
```

You can preview the production build with `npm run preview`.

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.

## Lessons Learned

1. Define components in `src/lib/components` folder, that's the preferred comunity project folder layout.
2. Export folder files in barrel files, so accessing them is easier (note: this doesn't affect performance, remember Svelte cuts everything that is not needed when bundling the app).
3. Define alias for main folders in `svelte.config.js` and then access them via **@** annotation (e.g., '@components': path.resolve('./src/lib/components/index.ts'))

## Tooling

Requires following tools:

- Node.js `v18.12.1`
- NPM `8.19.2`