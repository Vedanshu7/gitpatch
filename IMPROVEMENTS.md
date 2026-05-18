# gitpatch — Improvement Roadmap

## Near-term

- **Edit author name/email** — extend beyond just date changes to full commit metadata editing
- **Batch edit** — apply a date shift to a range of commits at once
- **Preview diff** — show what the commit log will look like before applying

## Cross-platform

- **macOS / Linux builds** — use Electron Forge to build `.dmg` and `.AppImage` packages
- **Auto-updater** — check for new releases on startup using `electron-updater`

## Security

- **Enable `contextIsolation`** — harden the Electron renderer process
- **Disable `nodeIntegration`** — use IPC bridge instead of direct Node.js access in renderer
- **Code signing** — sign Windows installer to avoid SmartScreen warnings

## Architecture

- **Migrate Bower → npm** — Bower is deprecated; move all frontend dependencies to npm
- **Electron Forge** — replace manual packaging with Electron Forge for consistent build pipeline
- **GPG signing support** — re-sign amended commits with GPG key
