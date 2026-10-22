# Cardinal GitHub Copilot CLI plugin

> [!NOTE]
> This repository is a **release mirror**. Development happens in
> [cardinal-agent-plugins](https://github.com/cardinalhq/cardinal-agent-plugins) — send PRs there.


This repository publishes one GitHub Copilot CLI plugin, `cardinal`, and is also its plugin marketplace (`.github/plugin/marketplace.json`).

The plugin source lives at [`plugins/cardinal`](./plugins/cardinal).

## Install

```bash
copilot plugin marketplace add cardinalhq/cardinal-copilot-plugin
copilot plugin install cardinal@cardinal-copilot-plugin
```

Then connect, with the plugin's `cardinal-connect` skill in a Copilot CLI session or in your own terminal:

```bash
python3 ~/.copilot/installed-plugins/cardinal-copilot-plugin/cardinal/scripts/cardinal-connect
```

The connect script runs Cardinal's browser-approved device-code flow and writes the managed `cardinal` and `cardinal-behavior` entries to `~/.copilot/mcp-config.json`. The plugin's hooks ship with the plugin and stay silent until you connect. Start a new Copilot CLI session (or `/restart`) afterwards; `copilot plugin update cardinal` picks up later releases.

See the plugin README for full behavior and options:

- [`plugins/cardinal/README.md`](./plugins/cardinal/README.md)

## License

Apache 2.0. See [LICENSE](./LICENSE).
