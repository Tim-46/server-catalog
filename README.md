# Server catalog

A list of dedicated game servers that can be installed with SteamCMD: App ID, name, platforms, download size, start command and the matching game (for the cover image).

The file `servers.json` is generated automatically and updated weekly. The app downloads it from here and falls back to its built-in copy when this file cannot be reached.

## Format

```json
{
  "version": 1,
  "generatedAt": "2026-11-03T11:54:24.093Z",
  "servers": [
    {
      "appId": 294420,
      "name": "7 Days to Die Dedicated Server",
      "os": ["windows", "linux"],
      "size": { "win32": 17896545174, "linux": 17803449012 },
      "launch": { "win32": { "executable": "startdedicated.bat", "args": "" } },
      "anonymous": true,
      "gameAppId": 251570
    }
  ]
}
```

- `appId`: Steam App ID of the dedicated server.
- `os`: platforms the server is available for.
- `size`: download size in bytes per platform, if known.
- `launch`: start command per platform, if known.
- `anonymous`: `true` if the server can be downloaded without a Steam account, `false` if an account is needed; missing if unknown.
- `gameAppId`: Steam App ID of the game itself.

## Contributions

This repository is updated automatically. Pull requests and issues are not accepted here.

## License

See [LICENSE](LICENSE) and [NOTICE](NOTICE). Game and server names are trademarks of their respective owners. This catalog is not affiliated with or endorsed by Valve or the game publishers.
