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
  sandbox devices.
  Source: [`inanimate-tech/resident`](https://github.com/inanimate-tech/resident/tree/main/tools/agent-plugin)
  (tracks `main`)

## Layout

```
.claude-plugin/
└── marketplace.json   # Claude Code marketplace catalog (name: inanimate)
```

Each plugin lives in its own product/system repo under `tools/agent-plugin/`
and is referenced from this marketplace via `git-subdir`. Skills are the
portable centre of gravity; tool-specific manifests are thin wrappers.

Cross-tool support (e.g. Codex) will be added by mirroring `marketplace.json`
under sibling directories like `.agents/plugins/` once those formats stabilise.

## Related

- Private/internal plugins live at
  [`inanimate-tech/agent-plugins-internal`](https://github.com/inanimate-tech/agent-plugins-internal)
  (marketplace name: `inanimate-internal`).
