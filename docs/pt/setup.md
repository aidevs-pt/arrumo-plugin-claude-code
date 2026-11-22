# Configura Claude Code no Arrumo

[English](../en/setup.md) · [Español](../es/setup.md)

Instala a CLI local e inicia sessão seguindo o [guia do fornecedor](https://code.claude.com/docs/en/setup). Inicia o Arrumo num ambiente cujo PATH inclua a pasta do executável.

Escolhe Claude Code durante a configuração do espaço de trabalho ou seleciona-o como agente de produção nas Definições. A verificação confirma a sessão local e não inicia uma edição.

## Verifica a ligação

Na CLI do editor, indica o caminho para uma base de dados local e o identificador deste plugin.

```sh
arrumo-workspaces ./workspaces.sqlite agent-login-status claude-code
```

O estado confirmed indica que a CLI aceitou a verificação. Se o Arrumo devolver unavailable, verifica se o executável está no PATH que o Arrumo consegue ver. Se devolver unconfirmed, inicia sessão seguindo o guia oficial e volta a verificar. Um tempo de espera excedido ou um erro indica que a verificação não foi concluída.

## Traduz as legendas

Consulta [a tradução de legendas](../../README.md#translate-subtitles) para usares este plugin como tradutor do Auto-Dubbing. O tradutor envia para Claude Code o texto das legendas selecionadas e o idioma de destino. O processo preserva as marcas temporais originais.

## Perguntas de seguimento

Quando o Claude Code pede ao Arrumo material do espaço de trabalho, como o guião de um vídeo anterior, o Arrumo responde na mesma sessão do Claude Code só com esse material, para que o pedido não seja enviado nem pago duas vezes. Estas sessões ficam no histórico do Claude Code (`claude --resume`); as execuções pontuais não guardam nenhuma.
