# Inanimate agent plugins

Public marketplace of agent plugins and skills for Inanimate developer tools
and devices.

## Installing

In Claude Code:

```
/plugin marketplace add inanimate-tech/agent-plugins
/plugin install <plugin>@inanimate
```

## Plugins

- **resident** — Skills for building, debugging, and extending Resident ESP32
  sandbox devices, at [`plugins/resident/`](plugins/resident/). For the
  Resident platform itself, see
  [`inanimate-tech/resident`](https://github.com/inanimate-tech/resident).

## Layout

```
.claude-plugin/
└── marketplace.json   # Claude Code marketplace catalog (name: inanimate)
plugins/
└── resident/          # One subdir per plugin
```

Plugins live in this repo under `plugins/` and are referenced from the
marketplace catalog by relative path.

Cross-tool support (e.g. Codex) is planned.

## Related

- Private/internal plugins live at
  [`inanimate-tech/agent-plugins-internal`](https://github.com/inanimate-tech/agent-plugins-internal)
  (marketplace name: `inanimate-internal`).
