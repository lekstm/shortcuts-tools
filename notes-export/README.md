# Notes Export Shortcut

Instructions for building a `.shortcut` file from `notes-export.cherri`.

## 1. Download Cherri

Download or build Cherri https://cherrilang.org and place the binary somewhere convenient, for example:

```bash
./cherri
```

Check that Cherri runs:

```bash
./cherri --version
```

## 2. Compile the Shortcut

```bash
./cherri /path/to/notes-export.cherri \
  --output=notes-export.shortcut
```

## 3. Open in Shortcuts

```bash
open /path/to/notes-export.shortcut
```

After opening it, add the shortcut to the Shortcuts app.

## What the Shortcut Does

- Finds Apple Notes notes.
- On first use, add a `Folder` filter manually and select the Apple Notes folder you want to export from.
- Sorts notes by `Creation Date`, newest first.
- Combines the contents of the selected Apple Notes folder into one file, including each note's creation and modification dates.
- Asks for an export name.
- Lets you save the result as `.txt` or `.md`.
- Creates a filename like `notes-export-folderName-20260404.md` or `notes-export-folderName-20260404.txt`.

The folder filter is intentionally not set in the code. You can add it manually in the first Shortcuts action with `+ Add Filter`.
