# NOTICE — origin & licensing

Storeforge is a rebranded ("white-labeled") build of:

- **Vendure** — https://github.com/vendure-ecommerce/vendure

`LICENSE.md` is retained.

## Licensing — GPLv3 (Community Edition)

Vendure is dual-licensed: **GPLv3** (Community Edition, the default) or a paid **Vendure
Commercial License (VCL)**. This clone uses the default **GPLv3**.

What GPLv3 requires of Storeforge:
- ✅ You may modify, rebrand, and self-host it.
- ✅ You must keep it under **GPLv3** and retain `LICENSE.md`.
- ⚠️ If you **distribute** it (ship the code/app to others), you must provide the complete
  corresponding source under GPLv3. (Note: GPLv3 — unlike AGPL — does **not** trigger purely
  from running it as a network service; distribution is the trigger.)
- ❌ You may not relicense it as closed-source. For a proprietary product, buy the VCL.

## How this rebrand was done (the sanctioned way)

Vendure provides **official white-label config** — no source hacking needed:

```ts
AdminUiPlugin.init({
  adminUiConfig: {
    brand: 'Storeforge',
    hideVendureBranding: true,
    hideVersion: true,
  },
})
```

Set in `packages/dev-server/dev-config.ts`. In your own project, set the same on your
`AdminUiPlugin` config. To finish the brand, also replace the admin logo asset
`packages/admin-ui/.../assets/logo-login.webp` and the favicon.
