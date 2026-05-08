# HUB EFCT — Template de Entrega de Ferramenta

Este repositório contém um pacote mínimo para criação e handoff de ferramentas no padrão do HUB EFCT.

## Arquivos principais

- `index.html`: template de front-end em HTML/CSS/JS vanilla com identidade visual EFCT.
- `HUB_METADATA.template.json`: modelo obrigatório para cadastro no HUB.
- `CHECKLIST_ENTREGA.md`: checklist obrigatório de validação antes da entrega.

## Como usar

1. Copie e personalize `index.html` com os dados da ferramenta.
2. Preencha `HUB_METADATA.template.json` e salve como `HUB_METADATA.json`.
3. Marque todos os itens em `CHECKLIST_ENTREGA.md`.
4. Faça deploy (Vercel para Opção A; Render para Opção B com backend Flask).

## Perguntas obrigatórias de intake (antes do desenvolvimento)

1. Nome da ferramenta
2. Descrição curta
3. Área responsável
4. Tipo de acesso (Interno/Externo)
5. Ícone (emoji Unicode)
6. Backend necessário? (Opção A ou B)
7. Nome de quem está desenvolvendo
