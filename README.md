# unblock-games-assets

Runtime assets served over `cdn.jsdelivr.net` / `raw.githubusercontent.com` / `unpkg` for a private parent project.

This repo exists only to host publicly-fetchable JSON and encrypted payloads. There is no source code here and issues / PRs opened against this repo will be closed without response.

## Contents

```
Technical Stuff/
├── config.json            # Remote config (passwords, blocked games, IP lists, minFileVersion)
├── game-data/             # AES-256-GCM encrypted game HTML payloads (.enc.json)
├── ip-log.json            # Append-only IP access log written by the auth server
├── panel-registry.json    # Self-registered admin panel list
└── config-pkg/            # npm package source (published as @pycoder42/ug-config for unpkg fallback)
```

## CDN endpoints

- jsDelivr: `https://cdn.jsdelivr.net/gh/PyCoder42/unblock-games-assets@latest/Technical%20Stuff/config.json`
- GitHub raw: `https://raw.githubusercontent.com/PyCoder42/unblock-games-assets/main/Technical%20Stuff/config.json`
- unpkg (via npm): `https://unpkg.com/@pycoder42/ug-config@latest/config.json`
