# pi-landstrip

Landlock-based sandboxing for [pi](https://pi.dev/) using
[`landstrip`](https://github.com/jarkkojs/landstrip).

## Prerequisites

Install `landstrip` and make sure it is on the `PATH` used to launch pi:

```bash
cargo install landstrip
```

`landstrip` supports Linux, macOS, and Windows. On other platforms this extension loads
but leaves sandboxing disabled.

## Install

```bash
pi install npm:pi-landstrip
```

## Configure

Create `.pi/sandbox.json` in a project or `~/.pi/agent/sandbox.json` globally.
Project config takes precedence.

See [`sandbox.json`](./sandbox.json) for a starter config.

## Usage

```bash
pi --no-sandbox
```

Use `/sandbox` inside Pi to show the active config.

## License

`pi-landstrip` is licensed under `MIT`. See [LICENSE](LICENSE) for more
information.
