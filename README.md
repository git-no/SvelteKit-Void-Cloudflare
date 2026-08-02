# SvelteKit-Void-Cloudflare Template

**Fast and simple SvelteKite deployment to Cloudflare.**

Template to deploy **SvelteKit** easily to **Cloudflare** and use Cloduflare resources within the SvelteKit app by Void adapter.

> Void is currently in Private Beta. We do not recommend using it for mission-critical production workloads yet. Please back up your data regularly.

### Repository contains

- [SvelteKit 2 (Svelte 5)](https://svelte.dev)
- [TailwindCSS](https://tailwindcss.com)
- [Void](https://void.cloud) - Ship Vite apps at warp speed

[Supported Void App Types](https://void.cloud/guide/app-types#void-apps): Vite apps powered by Void's framework layer, including [API routes](https://void.cloud/guide/server-routing), [pages mode](https://void.cloud/guide/pages-routing/overview), [auth](https://void.cloud/guide/auth) - [better-auth](https://better-auth.com) support, [crons](https://void.cloud/guide/jobs), and [queues](https://void.cloud/guide/queues)

## Demo

See this repository live at [Cloudflare]()

## Start

1. Clone this repository
2. Install packages in the repository directory by using `pnpm i`
3. Change the app name in `wrangler.jsonc` file.
4. Deploy to Cloudflare by
    - `void auth login`  
    (if you get the error `command not found: void`, then void is installed as local package, not global. Use `pnpm void auth login` instead)
    - `void deploy`

## References

[Using Void Platfrom Features in SvelteKit](https://void.cloud/integrations/frameworks/sveltekit#using-void-platform-features)

[Void SvelteKit Integrations](https://void.cloud/integrations/frameworks/sveltekit)

[Deployment](https://void.cloud/guide/deployment)

SvelteKit uses Vite internally with its own Cloudflare adapter (`@sveltejs/adapter-cloudflare`). The `voidPlugin()` in the Vite config handles binding inference, typed DB, and migrations during development.
