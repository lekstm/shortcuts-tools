# meow IP Shortcut

Instructions for building a `.shortcut` file from `meow-ip.cherri`.

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
./cherri /path/to/meow-ip.cherri \
  --output="meow IP.shortcut"
```

## 3. Open in Shortcuts

```bash
open "/path/to/meow IP.shortcut"
```

After opening it, add the shortcut to the Shortcuts app.

## What the Shortcut Does

- Gets your public external IP address from `https://api.ipify.org`.
- Shows a macOS notification with the shortcut name, a blank line, and your IP address.
- Adds a random cat face emoji before the IP address in the notification.
- Copies the IP address to the clipboard.
- Sets the clipboard item to expire after 10 minutes.
