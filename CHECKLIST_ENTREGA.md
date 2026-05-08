# Checklist de entrega — HUB EFCT

> Use este checklist **antes de entregar** a ferramenta ao Ricardo (ricardo@efct.com.br).
> Se algum item falhar, volte e corrija. Não entregue parcial.

## Funcionalidade
- [ ] URL de produção está acessível publicamente (teste numa janela anônima)
- [ ] Todas as funções principais da ferramenta funcionam do começo ao fim
- [ ] Mensagens de erro são humanas (não mostram stack trace cru pro usuário)
- [ ] Se consulta CNPJ: usa BrasilAPI com fallback CNPJa e `User-Agent` correto
- [ ] Se gera `.docx`/`.pdf`: arquivo baixa corretamente e abre sem erros

## Padrão visual EFCT
- [ ] Header escuro `#1F2937` com "HUB EFCT | [Nome da Ferramenta]"
- [ ] Link "voltar ao HUB" apontando para `https://effect-contratos-api.onrender.com`
- [ ] Paleta de cores EFCT aplicada (azul `#3B82F6`, fundo `#F3F4F6`, cards `#FFFFFF`)
- [ ] Fonte sistema nativa (`-apple-system, BlinkMacSystemFont, 'Segoe UI'`)
- [ ] Cards com `border-radius: 12px` e sombra sutil
- [ ] Botões primários azul EFCT
- [ ] Testado em mobile (responsive) — ao menos layout não quebra

## Código
- [ ] Frontend em **um único `index.html`** inline, sem frameworks
- [ ] Se Opção B: `Dockerfile`, `requirements.txt` e `render.yaml` presentes
- [ ] `BASE_DIR = os.path.dirname(os.path.abspath(__file__))` — sem paths absolutos
- [ ] Sem credenciais/chaves hardcoded no código (variáveis de ambiente)
- [ ] `.gitignore` cobrindo `.env`, `__pycache__`, `outputs/`, etc

## Documentação
- [ ] `README.md` na raiz explicando o que a ferramenta faz e como rodar
- [ ] Se tem login próprio: credenciais de teste documentadas no README

## Pacote de handoff (o que enviar pro Ricardo)
- [ ] URL de produção (funcional)
- [ ] `HUB_METADATA.json` preenchido (todos os campos não-null)
- [ ] Screenshot PNG/JPG da tela principal
- [ ] Relatório de entrega formatado (modelo na Seção 7.4 das instruções)
- [ ] `validacoes.*` no JSON: todos os campos marcados como `true`

## Checagem final
- [ ] Reabri a URL num navegador sem cache e tudo funciona
- [ ] Conferi que o screenshot reflete a versão deployada mais recente
- [ ] Confirmei o emoji do ícone renderiza em macOS (não usar emojis muito novos)

---

**Se todos os itens acima estão marcados**, envie para ricardo@efct.com.br o pacote descrito no último grupo.
