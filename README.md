# timezone-dashboard

A standalone React UI component for a world timezone dashboard: shows live clocks for multiple cities/timezones side by side, with a timezone selector to add or change displayed zones. This is a drop-in component (React + shadcn/ui-style primitives) meant to be pasted into an existing React project — not a full standalone application.

## What's inside

| File | Description |
|------|-------------|
| `timezone-dashboard` | Timezone dashboard component: live per-zone clocks (`useEffect` + interval), timezone picker (`Select` from shadcn/ui), card-based layout |

The component imports React (`useState`, `useEffect`), `lucide-react` (`Clock`), and `@/components/ui/*` (shadcn/ui `button`, `card`, `label`, `select`) — and uses the browser `Intl.DateTimeFormat` / `toLocaleTimeString` time-zone support for conversions.

## Quick start

This file has no `package.json` — it is a component, not an app. To use it:

1. Copy the file into your React project's components folder (rename it without spaces, e.g. `TimezoneDashboard.tsx`).
2. Make sure your project has shadcn/ui components (`button`, `card`, `label`, `select`) and `lucide-react` installed.
3. Import and render the component like any other React component.

```bash
npm install lucide-react
```

## Tech stack

- React (hooks: `useState`, `useEffect`)
- shadcn/ui primitives (button, card, label, select)
- Tailwind CSS utility classes
- lucide-react icons
- Native `Intl` timezone formatting (no extra date library)

## Deploy notes

No deployment — this repository contains a source component only, not a runnable website. To ship it as a page, drop the component into a Vite/Next.js project and deploy that.

## License

CC0 1.0 Universal — see `LICENSE`.

---

Built by Girish Lade — https://ladestack.in
