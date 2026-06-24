# Rune

Rune is a macOS terminal emulator with a built-in Git graph, database browser, and a smarter input bar. It sits on top of a real PTY session so everything works exactly like a normal terminal, with extra tooling that appears when you need it.

<img width="1470" height="830" alt="Rune terminal with git graph and saved commands" src="https://github.com/user-attachments/assets/44b5e8d2-f0f4-4af8-a797-2bd661551cb0" />

## Input bar

Commands go through a dedicated input bar instead of directly into the terminal output. It has persistent history, path completion, and a slash-command palette for saved shortcuts. Type `/` to search and insert any saved command instantly. When Claude Code, vim, or similar tools take over, the bar steps aside and comes back when they exit.

<img width="843" height="228" alt="Slash command palette" src="https://github.com/user-attachments/assets/37cf2395-10fd-4aed-b265-f8d365819645" />
<img width="1167" height="155" alt="Screenshot 2026-06-24 at 11 28 02 PM" src="https://github.com/user-attachments/assets/7aabfbd5-2c38-49e7-9c34-275ad8778586" />

## Database browser

Detects active mysql and psql sessions automatically. A schema tree appears in the sidebar with no setup required. Click any table to see its data in a full-width results grid. Runs on a background connection so the terminal session is never interrupted.

<img width="1470" height="956" alt="Database browser with schema tree and query results" src="https://github.com/user-attachments/assets/5926b2a4-20c3-4db5-9017-3947aef5cdfc" />



## Git graph

Opens automatically in git repos. Shows branch history with colored lanes, ref pills, and expandable commit details. Fetch from remote with one click.

## Everything else

- **Saved commands** — collections of commands, searchable with /, import and export as JSON
- **SSH profiles** — save and launch SSH connections from the tab bar
- **Session persistence** — tabs reopen in their previous working directories
- **Status bar** — git branch, dirty file count, Node version, active venv, last exit code

## Install

macOS only (Apple Silicon and Intel).

Download the latest `.dmg` from the [Releases](../../releases) page, open it, and drag Rune to your Applications folder.

## Tech

Electron, Vite, React, node-pty, xterm.js.

## License

MIT
