# Lindows OS

Lindows OS is an original desktop environment simulation built with React, TypeScript, Vite, Tailwind CSS, and Lucide. It runs in a browser and does not require an account.

## Run locally

```sh
npm install
npm run dev
```

`npm run build` runs the TypeScript project checks and creates a production build. `npm run lint` runs Oxlint.

## Design direction

The desktop uses a soft-pastel palette with a crisp system sans, abstract wallpaper, quiet borders, and short motion that confirms window and panel changes. The desktop is the work surface; applications use shared window chrome and semantic light/dark tokens. Accent color and wallpaper are user-selectable.

## Included applications

- **Files** — virtual Home folders and documents; create, rename, move, and delete items.
- **Notes** — create and edit notes with automatic local saving.
- **Calculator** — arithmetic with operator precedence, keyboard input, and backspace.
- **Settings** — theme, wallpaper, accent, desktop shortcuts, clock, and taskbar options.
- **System Information** — version and clearly identified simulated hardware details.
- **Browser** — bookmarks and search/address controls that open external pages in regular browser tabs.
- **Terminal** — safe simulated `help`, `clear`, `date`, `version`, `ls`, and `echo` commands only.
- **Control Center** — local theme, taskbar, connectivity, brightness, and volume-style controls.
- **Devlogs** — illustrative project stages, explicitly not a historical record.

## Desktop controls

- Drag a title bar to move a window; drag an edge or corner to resize.
- Double-click a title bar to maximize or restore. Use the title-bar buttons to minimize, maximize, or close.
- Drag a window to the left or right screen edge to snap it to half the desktop.
- Select a running taskbar icon to focus or minimize its window.
- Right-click the desktop for shortcuts and reset options.
- `Ctrl+Alt+Space` opens the launcher, `Ctrl+Alt+T` opens Terminal, `Ctrl+Alt+←/→` snaps the focused window, `Alt+F4` closes it, and `Escape` closes open panels.

## Browser boundaries and data

The terminal, hardware information, connectivity, brightness, and volume controls are simulations; they do not access or change the host operating system. The browser app uses ordinary browser tabs and security rules rather than embedding unrestricted pages.

Preferences, notes, and the virtual filesystem are stored in this browser profile with localStorage. No account or authentication is used. If browser storage is unavailable or full, Lindows shows a persistent warning. Reset restores the default settings and virtual files and removes saved notes.
