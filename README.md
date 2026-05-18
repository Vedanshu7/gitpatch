# gitpatch

> Edit the timestamp and author of any past git commit — via a simple GUI.

`gitpatch` is a Windows desktop application (built with Electron) that lets you select any commit in your repository and change its author date or committer date, without touching the command line.

> **Warning:** Changing commit metadata rewrites history. You will need to force-push to remote, which will require all collaborators to re-pull. Use on personal repos or with team agreement.

## Features

- Browse all commits in a local git repository
- Select any commit and change its date/timestamp
- Clean GUI — no need to memorise `git filter-branch` commands
- Works with any git repository on Windows

## Requirements

- **Windows** (the `.exe` installer)
- **Git** must be in your PATH (e.g. `C:\Program Files\Git\bin`)

## Installation

1. Download `Setup.exe` from [Releases](https://github.com/Vedanshu7/gitpatch/releases)
2. Run the installer
3. Open **gitpatch** from the Start Menu or Desktop

## Usage

1. Click **Open Repository** and navigate to your local git repo
2. Select the commit you want to edit from the list
3. Change the date/time fields
4. Click **Apply** — gitpatch rewrites the commit locally
5. Force-push to remote: `git push --force origin main`

## Example

**Before:**
```
Commit abc123 — Dec 2 08:08:21 2021
```
**After (date changed to Jul 6):**
```
Commit abc123 — Jul 6 08:08:21 2021
```

## License

MIT
