# 🗺 Cartograph Studio

A free, open-source map poster and wallpaper creator. Design beautiful, print-ready map art for any city or location — no sign-up required.

## Features

- 🌍 Search any city or location worldwide
- 🎨 6 theme presets + full custom color control per map layer
- ✍️ Draggable, editable text blocks
- 🖼 Frame styles (thin, double, corner marks, ornate)
- 📤 Export as PNG, JPG, PDF, or SVG
- 🔍 Quality options: Web → HD → Print (300dpi) → Ultra (600dpi)
- No login, no backend, runs 100% in the browser

## Getting Started

Just open `mapposter.html` in any modern browser. No build step, no dependencies to install.

## Optional: Mapbox Styles

By default, the app uses free OpenStreetMap raster tiles — no API key needed.

If you want to use Mapbox vector styles (for sharper per-layer color control):

1. Create a free account at [mapbox.com](https://mapbox.com)
2. Copy your **public** token (starts with `pk.`)
3. In `mapposter.html`, find this line and replace the placeholder:

```js
mapboxgl.accessToken = 'YOUR_MAPBOX_TOKEN';
```

> ⚠️ Never commit a real Mapbox **secret** token (starts with `sk.`) to a public repo.  
> Public tokens (`pk.`) are safe to commit but you can also keep them in a `.env` file.

## Roadmap

- [ ] User accounts & saved designs
- [ ] Server-side high-resolution rendering (Node.js + Puppeteer)
- [ ] More map style presets
- [ ] Premium export options

## License

MIT — free to use, modify, and distribute.

## Credits

- Map data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright) (ODbL)
- Location search via [Nominatim](https://nominatim.org/)
- Rendered with [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/)
