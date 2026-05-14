<div align="center">

<img src="https://raw.githubusercontent.com/openlid/open-lid/main/resources/branding/openlid-org-avatar.png" alt="Open-Lid" width="120" height="120" />

# Open-Lid

**Tools that keep your laptop out of your way.**

</div>

We build small, focused utilities that respect your machine. Native UI
where possible. No telemetry. No data leaves your machine. Apache 2.0
licensed.

Targeting **macOS today**, **Linux planned for v1.x**, **Windows on demand**
behind a platform-abstraction layer in pure Rust.

## Projects

### [open-lid](https://github.com/openlid/open-lid)

> Keep your laptop awake — even with the lid closed.

A small utility that prevents your laptop from sleeping when you close
the lid (and from dimming when the lid is open). Single-digit megabyte
binary, signed and notarized for macOS distribution.

```bash
# macOS (today):
brew install --cask openlid/tap/open-lid

# Linux + Windows: planned (see project roadmap).
```

[Latest release →](https://github.com/openlid/open-lid/releases/latest) ·
[Documentation →](https://github.com/openlid/open-lid#readme) ·
[Architecture →](https://github.com/openlid/open-lid/blob/main/docs/ARCHITECTURE.md)

## Principles

- **Native, not Electron.** Rust everywhere, with native UI bindings per
  platform (AppKit on macOS via `objc2`, planned GTK/Qt on Linux).
  Single-digit megabyte binaries. Cold-launch in under a second.
- **No telemetry. No analytics. No automatic update checks.** Your
  machine is yours. We don't even know who's using our software, and
  we like it that way.
- **Source available, source clean.** All code published under Apache 2.0.
  Read it, fork it, improve it, redistribute it.
- **Small, focused tools.** Each app does one thing well. We resist
  feature creep so the utilities stay easy to understand and easy to
  trust.
- **Cross-platform by design, not by accident.** Pure-Rust core crates
  (state machines, IPC schemas, config) compile on every target; only
  the thin OS-binding layer changes per platform.

## Contributing

Each repo has its own `CONTRIBUTING.md`. The short version:

- Bug fixes welcome any time.
- New features should go through an issue first so we can align on
  the design before you write code.
- Linux/Windows backend contributions are very welcome **after** v1.0
  of any given project — porting before the platform-traits stabilize
  is wasted work.
- Issues and PRs are triaged in spare time — please be patient.

## License

Apache 2.0 across all projects unless explicitly noted.
