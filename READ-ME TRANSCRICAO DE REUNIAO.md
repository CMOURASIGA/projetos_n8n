# Automação de Atas de Reuniões Teams com n8n, Microsoft Graph e Azure OpenAI

Este projeto tem como objetivo automatizar a captura, tratamento e organização de transcrições de reuniões do Microsoft Teams, gerando arquivos estruturados de resumo, ata e metadados para armazenamento no OneDrive ou SharePoint.

A solução foi construída em n8n, utilizando Microsoft Graph para acesso a calendário, reuniões online, transcrições e arquivos, além de Azure OpenAI para geração dos conteúdos em Markdown.

---

## 1. Objetivo do projeto

Automatizar o processo de geração de atas a partir de reuniões realizadas no Microsoft Teams.

O fluxo busca reuniões no calendário do usuário ou de usuários monitorados, localiza a reunião online correspondente, baixa a transcrição, processa o conteúdo com IA e salva os arquivos resultantes em uma estrutura organizada.

Arquivos gerados por reunião:

```text
YYYY-MM-DD - Ata da Reuniao - Nome.md
01 - Resumo Geral.md
02 - Resumo por Orador.md
03 - Transcricao.md
metadados-reuniao-YYYY-MM-DD.json