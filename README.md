# SvelteKit + Supabase Starter

[still in progress, just some basic docs for now]

This is simple, barebone starter template for SvelteKit with Supabase. Work in progress.
There is authentication with email and password and OAuth with Github.

## Getting started

To get started you can clone this repository or use 'Use this template' button.

After cloning the repository install the dependencies:

```bash
bun install
```

If you want to use Supabase locally make sure to follow these instructions: https://supabase.com/docs/guides/local-development. You can start your server with

```bash
bun supabase:start
```

and stop it with

```bash
bun supabase:stop
```

You can also just create your instnce on supabase.com and use it.

After you have your Supabase instance you need to create a `.env` and fill it like in the `.env.example` file.
You can omit Github OAuth stuff if you do not want to use it.
