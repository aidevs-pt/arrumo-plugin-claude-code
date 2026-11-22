# Arrumo Claude Code Plugin

The Claude Code agent adapter for planning, executing, and reporting on Arrumo video jobs.

## Icon and trademarks

`icon.svg` uses the official Claude Code mark, only to identify the service this
plugin connects to. Claude, Claude Code and their logos are trademarks of Anthropic. This plugin is not affiliated with or endorsed by
Anthropic, and the mark is not covered by this repository's license.

Copyright © 2026 DEVS AI Unipessoal LDA. Licensed under the [GNU Affero General Public License v3.0](LICENSE).

For custom AI solutions for your company, visit [DEVS AI](https://aidevs.pt).

The manifest declares the provider label, setup guide, and local authentication status command through the Arrumo Plugin SDK. The plugin ID is `claude-code`.

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
