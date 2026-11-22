# Arrumo Claude Code Plugin

The Claude Code agent adapter for planning, executing, and reporting on Arrumo video jobs.

## Icon and trademarks

`icon.svg` shows Anthropic's logo so creators recognise the service this plugin connects to. Claude, Claude Code and their logos are trademarks of Anthropic; the manifest's `iconNotice` says so wherever Arrumo shows the icon. The logo is not covered by this repository's license, and this plugin is not affiliated with or endorsed by Anthropic. The SVG is a square without rounded corners; Arrumo rounds it. If Anthropic asks, replace the logo with a generic symbol and remove `iconNotice`.

## Setup guide

[English](docs/en/setup.md) · [Español](docs/es/setup.md) · [Português](docs/pt/setup.md)

## Translate subtitles

Use `tools/translate-subtitles.py` as Auto-Dubbing's local translator. It
uses the existing Claude Code login, sends cue text and the target language,
and checks that the structured response includes exactly one translation per
cue. Use a CLI version that supports restricted mode and JSON schema output.

The adapter runs in a temporary directory and requests no built-in tools,
an empty MCP configuration, disabled hooks, and no session persistence.
[Claude Code headless reference](https://code.claude.com/docs/en/headless)
