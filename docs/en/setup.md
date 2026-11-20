# Set up Claude Code in Arrumo

[Español](../es/setup.md) · [Português](../pt/setup.md)

Install and sign in to the local CLI using the [provider setup guide](https://code.claude.com/docs/en/setup). Start Arrumo from an environment whose PATH includes the directory containing the CLI executable.

Choose Claude Code during workspace setup or select it as the production agent in Settings. A sign-in check confirms local authentication. It does not start an edit.

## Check the connection

From the editor CLI, pass a local database path and this plugin ID.

```sh
arrumo-workspaces ./workspaces.sqlite agent-login-status claude-code
```

A confirmed status means the CLI accepted the sign-in probe. If Arrumo reports unavailable, check that the executable is on the PATH visible to Arrumo. If the login is unconfirmed, sign in using the official guide and check again. A timeout or failure means the probe could not finish successfully.

## Translate subtitle cues

See [Translate subtitles](../../README.md#translate-subtitles) to use this plugin as an Auto-Dubbing translator. The translator sends the selected cue text and target language to Claude Code. The workflow keeps the original cue timings.
