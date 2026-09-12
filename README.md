# Forge CRM

Forge CRM is a static, mock-data CRM workspace for reviewing leads, financial records, communications, documents, and dialer interactions. It runs entirely in the browser and does not connect to a production CRM, phone service, messaging provider, or authentication service.

## Run locally

From the project directory, start a static server:

```bash
python3 -m http.server 4173 --bind 0.0.0.0
```

Then open [http://127.0.0.1:4173/](http://127.0.0.1:4173/).

## GitHub Pages

The public deployment is available at [https://antonio3055.github.io/manuscrm/](https://antonio3055.github.io/manuscrm/). GitHub Pages is configured from the `main` branch.

## Navigation and Settings

The default navigation is the Main 5-inspired top bar. Settings also supports compact sidebar icons and a wide text sidebar. Settings preferences persist in browser local storage and include panel density, financial-summary visibility, default communications tab, theme choice, motion, screen scale, font size, and panel-width reset.

## Keyboard shortcuts

| Shortcut | Action |
| --- | --- |
| `/` | Focus CRM search |
| `K` | Toggle the dialer keypad |
| `C` | Call the selected lead |
| `Enter` | Start a call from the dialer |
| `Esc` | Close overlays, search, keypad, or dialogs |
| `←` / `→` | Move through document pages when a viewer is open |

## Project structure

The `index.html` entry point loads the shared shell, CRM renderers, mock data, and active styles. Core styles are in `css/base.css`, `css/shell.css`, `css/crm.css`, `css/communications.css`, and the consolidated `css/forge-final.css`. Page-specific HTML files live in `pages/`.

## Mock-data disclaimer

All leads, financial values, contacts, statements, messages, and call records are demonstration data intended for UI testing and design review only.
