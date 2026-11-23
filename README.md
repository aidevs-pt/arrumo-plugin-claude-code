<p align="center">
  <img src="icon.svg" width="88" height="88" alt="">
</p>

<h1 align="center">Claude Code for Arrumo AI Video Editor</h1>

<p align="center">Use Claude Code as the agent that writes, designs and cuts your videos in Arrumo, on your own Claude plan.</p>

<p align="center">
  <a href="LICENSE"><img alt="License: AGPL-3.0" src="https://img.shields.io/badge/license-AGPL--3.0-2337B4"></a>
  <img alt="Bundled with Arrumo" src="https://img.shields.io/badge/bundled%20with-Arrumo-2337B4">
  <a href="https://www.aidevs.pt/tools/arrumo/docs/plugins/claude-code/setup"><img alt="Docs in English, Spanish and Portuguese" src="https://img.shields.io/badge/docs-EN%20%C2%B7%20ES%20%C2%B7%20PT-111"></a>
</p>

This plugin ships with [Arrumo AI Video Editor](https://github.com/aidevs-pt/arrumo-video-editor), the free, open-source desktop app where an AI agent writes, designs, voices and cuts your videos and you approve every step. It comes installed with Arrumo; turn it on or off in **Settings › Plugins**.

## Guides

- **Set up Claude Code**: [English](https://www.aidevs.pt/tools/arrumo/docs/plugins/claude-code/setup) · [Español](https://www.aidevs.pt/es/tools/arrumo/docs/plugins/claude-code/setup) · [Português](https://www.aidevs.pt/pt/tools/arrumo/docs/plugins/claude-code/setup)

## Translate subtitles

Use `tools/translate-subtitles.py` as Auto-Dubbing's local translator. It
uses the existing Claude Code login, sends cue text and the target language,
and checks that the structured response includes exactly one translation per
cue. Use a CLI version that supports restricted mode and JSON schema output.

The adapter runs in a temporary directory and requests no built-in tools,
an empty MCP configuration, disabled hooks, and no session persistence.
[Claude Code headless reference](https://code.claude.com/docs/en/headless)

## Icon and trademarks

`icon.svg` shows Anthropic's logo so creators recognise the service this plugin connects to. Claude, Claude Code and their logos are trademarks of Anthropic; the manifest's `iconNotice` says so wherever Arrumo shows the icon. The logo is not covered by this repository's license, and this plugin is not affiliated with or endorsed by Anthropic. The SVG is a square without rounded corners; Arrumo rounds it. If Anthropic asks, replace the logo with a generic symbol and remove `iconNotice`.

## License

Copyright © 2026 DEVS AI Unipessoal LDA. Licensed under the [GNU Affero General Public License v3.0](LICENSE). Built by [DEVS AI](https://aidevs.pt), who make custom AI solutions for companies.
