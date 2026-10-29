<h1 align="center">Colspan</h1>
<p align="center">Open source drag & drop builder for HTML emails that hold together in every inbox</p>
<img src="./hero.jpg">

<p align="center">
  <a href="https://colspan.dev/app">Live Demo</a>
  ·
  <a href="https://colspan.dev">Website</a>
  ·
  <a href="https://github.com/colspan-dev/colspan/releases">Releases</a>
  ·
  <a href="https://github.com/colspan-dev/colspan/discussions">Discussions</a>
</p>

> Colspan was previously called **MySigMail Card** and lived at `card.mysigmail.com`. Old links redirect here.

## Why Colspan

Email layout still runs on tables. Every email developer has fought nested `<table>`s, `colspan` and Outlook quirks. Colspan does that part for you: you assemble an email from ready-made blocks, and it produces table-based HTML with inline styles, built to render consistently across Gmail, Outlook and Apple Mail.

We live in an era of increasing vendor lock-in and centralized control. Entire regions get cut off from services for geopolitical reasons, leaving developers and users stranded. Software should be accessible and reliable regardless of borders. Colspan is the open core of my commercial email builder, released so that everyone has a powerful email editor they can host themselves.

## Features

- Visual drag-and-drop editor
- Component catalog with 78 ready-to-use blocks across **Menu**, **Header**, **Content**, **Feature**, **Call to Action**, **E-Commerce**, **Transactional**, and **Footer**
- Inline editing and a synchronized component tree (`Block -> Row -> Cell -> Atom`)
- Atom types: `text`, `button`, `divider`, and `image`; Menu and Social are reusable recipes built from the same primitives
- Rich-text editing with Google Fonts support
- Desktop and mobile preview with per-row stacking and mobile visibility controls
- Responsive HTML export and editable JSON export/import from the UI
- Import modes: `replace` and `append`
- Template validation + sanitization on import
- Auto-persist to `localStorage` and hydration on reload
- Undo and redo
- Preview rendered in Shadow DOM to isolate editor styles

## Self-hosting

Colspan is a static app: build it and serve `dist/` from any web server.

```sh
pnpm i
pnpm build
```

Environment variables (see `.env.example`):

| Variable | Purpose |
| --- | --- |
| `VITE_APP_BASE_PATH` | Base path the app is served from, e.g. `/app/` |
| `VITE_APP_TELEMETRY` | `true` enables analytics; leave empty for self-hosting |
| `VITE_APP_YM_ID` | Yandex Metrica counter id, used only with telemetry |

## Development

```sh
pnpm i
pnpm dev
```

Run checks with `pnpm lint` and `pnpm test`.

## Roadmap

The original codebase served well for years, but the web has evolved. I am rewriting the core from scratch with modern web standards and architectural patterns, so the project stays fast, maintainable, and easy to extend for years to come.

## Support

Colspan is an open source project and completely free to use.

However, the amount of effort needed to maintain and develop new features for the project is not sustainable without proper financial backing. You can support Colspan development via the following methods:

<div align="center">

[![Donate via Open Collective](https://img.shields.io/badge/donate-Open%20Collective-blue.svg?style=popout&logo=opencollective)](https://opencollective.com/mysigmail)
[![Donate via PayPal](https://img.shields.io/badge/donate-PayPal-blue.svg?style=popout&logo=paypal)](https://paypal.me/antongithub)

</div>

## How can I help?

Since the project is undergoing a major rewrite, architectural decisions are still in flux. Direct code contributions might be tricky at this stage, but I welcome feedback and discussions.

**The best way to help right now is to star the repository ⭐** and share it with others. Visibility helps the project grow!

![](./subscribe.gif)

## Follow

- News and updates on [Twitter](https://twitter.com/mysigmail).
- [Discussions](https://github.com/colspan-dev/colspan/discussions)

## Commercial Usage

This project is licensed under the **AGPL-3.0**. This means if you include this editor in your own software and make it available to users over a network (SaaS), you must also make your software open source under the same license.

**Need a commercial license?**

If you want to use this editor in a proprietary application without open-sourcing your code, please [contact me](mailto:reshetov.art@gmail.com) for a commercial license.

## License

[AGPL-3.0](LICENSE)

Copyright (c) 2022-present, Anton Reshetov.
