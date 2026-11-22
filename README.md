# Arrumo Claude Code Plugin

The Claude Code agent adapter for planning, executing, and reporting on Arrumo video jobs.

## Icon and trademarks

`icon.svg` is a generic symbol drawn for Arrumo (code brackets, for an agent that writes and reviews code), covered by this repository's
license. It is not the provider's logo: the provider has not published permission for its
logo to appear in another app's interface, so the plugin does not use it. The name is used
only to say which service the plugin connects to; this plugin is not affiliated with or
endorsed by the provider.

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
