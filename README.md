# Pioneer Bank — Modern Banking Landing & Demo

A polished, responsive single-page demo for a lightweight banking login/dashboard built with Tailwind CSS and DaisyUI. Designed to showcase a modern UI, micro-interactions, and a minimal client-side transaction demo.

## Live preview

- Open the demo in any modern browser: [index.html](index.html)

## Key features

- Clean, responsive layout with Tailwind CSS and DaisyUI.
- Animated hero illustration with graceful fallback.
- Toggleable authentication UI (Login / Signup) and a lightweight client-side account dashboard.
- Simple deposit/withdraw demo that updates on-page balances without a backend.
- Accessible controls and mobile-first design.

## Built with

- Tailwind CSS (via CDN)
- DaisyUI (via CDN)
- Font Awesome (icons)
- Vanilla JavaScript (no build step)

## Files of interest

- Project entry: [index.html](index.html)
- This document: [README.md](README.md)

## Implementation highlights (in [index.html](index.html))

- UI flow control:
  - [`show-signup`](index.html) and [`show-login`](index.html) — toggles between auth forms
  - [`login`](index.html) — transitions to the transaction dashboard
- Transaction demo (client-side):
  - Functions: [`getInputNumber`](index.html), [`updateSpanText`](index.html)
  - Controls / IDs: [`addDeposit`](index.html), [`addWithdraw`](index.html)
  - Live display IDs: [`currentDeposit`](index.html), [`currentWithdraw`](index.html), [`currentBalance`](index.html)

## Quick start

1. Clone or download this repository.
2. Open [index.html](index.html) in your browser (double-click or use a local static server).
   - Optional (recommended): serve via a simple static server for correct icon/CSP behavior:
     - Python 3: python -m http.server 8080
     - Node: npx serve .

## Usage notes

- The demo uses only client-side state (no authentication or persistence). It is ideal for prototyping UI/UX and presenting to clients.
- To reset the demo values, refresh the page.

## Customisation tips

- Tailwind theme colors can be edited in the inline Tailwind config at the top of [index.html](index.html).
- Replace the demo illustration URL or local asset in the hero image block.
- Swap icons or add more DaisyUI components to extend the dashboard or add real form validation.

## Developer notes

- The transaction logic is intentionally simple:
  - [`getInputNumber`](index.html) parses numeric inputs.
  - [`updateSpanText`](index.html) mutates visible totals.
- Consider adding persistence (localStorage or backend) and server-side authentication for production.

### Accessibility & performance

- Mobile-first responsive layout with semantic HTML.
- Minimal external dependencies (CDN) for quick demos — review privacy and CSP for production.

#### Contributing

- PRs and issues welcome. For UI changes, include before/after screenshots and a short description of behavior.

##### License

- MIT — feel free to reuse and extend.

###### Contact

- For portfolio / client demos, this page is ready to be professional.
