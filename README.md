# shortcuts-tools
macOS shortcuts application in code

Instructions for building a `.shortcut` file from `meow.cherri`.

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
./cherri /path/to/meow.cherri \
  --output="meow.shortcut"
```

## 3. Open in Shortcuts

```bash
open "/path/to/meow.shortcut"
```

After opening it, add the shortcut to the Shortcuts app.