# create-svelte with Cloudflare using `bun`.

Everything you need to build a Svelte project, using `bun` and powered by [`create-svelte with cloudflare`](https://developers.cloudflare.com/pages/framework-guides/deploy-a-svelte-site/).

## Creating a project

If you're seeing this, you've probably already done this step. Congrats!

There are two ways to go about this. It is really a personal preference.

The following command will create a new directory called `afrotest` and build the project in it.

```bash
# create a new project in the current directory
bun create cloudflare@latest afrotest -- --framework=svelte
```

This command will create new project in the directory called `afrotest` and ask you to create a new name for the Svelte app.

```bash
# create a new project in a directory called afrotest
bun create cloudflare@latest -- --framework=svelte
```

## Developing

Once you've created a project and installed dependencies with `npm install` (or `pnpm install` or `yarn`), start a development server:

```bash
bun run dev

# or start the server and open the app in a new browser tab
bun run dev -- --open
```

## Building

To create a production version of your app:

```bash
bun run build
```

You can preview the production build with `bun run preview`. This is important since it helps you catch errors that are not showing up in `dev`.

## Deploying

> To deploy your app, you may need to install an [adapter](https://kit.svelte.dev/docs/adapters) for your target environment.
> Fortunately, if you installed with `bun`, this step is taken care of. Navigate to the new directory:

```bash
cd afrotest

# Run the development server
bun run pages:dev

# Deploy your application
bun run pages:deploy
```

Read the documentation https://developers.cloudflare.com/pages
