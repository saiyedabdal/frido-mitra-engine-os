# Frido Mitra — Engine OS

Single-file static command dashboard for **Frido's affiliate program** (Project: Frido Mitra / Buddy / Ambassador). It visualizes the program's operating model: **9 sequential macro engines** (E1 Acquiring → E9 Retention) executed per affiliate channel.

🌐 **Live:** https://frido-mitra-engine-os.netlify.app

## Views
- **Dashboard** — each channel as a 9-station "engine line"; KPI cards; POC markers; show-stopper feed.
- **Registry** — AC/SAC channel tree, legacy L1–L4 mapping, per-channel rollups.
- **Cockpit** — one channel end-to-end across E1–E9, with coverage gaps called out.
- **Lens** — one engine across all channels; stacked status bars.

## Stack
Pure static — one `index.html`, vanilla JS, hash router, **no build step**. Fonts via Google Fonts (Bricolage Grotesque · Instrument Sans · IBM Plex Mono). Dark "control-room" theme where the status spectrum carries meaning (slate → saffron → sky → jade, ember = stoppers).

## Deploy
Hosted on Netlify (publish dir `.` per `netlify.toml`). The `main` branch is connected for continuous deployment — pushes build and publish automatically.

```bash
# manual deploy (fallback)
netlify deploy --prod
```

See [`CLAUDE.md`](CLAUDE.md) for the operating model and [`docs/engine-os-design.md`](docs/engine-os-design.md) for the full system design (schema, views, 14-day plan).
