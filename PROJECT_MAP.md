# PROJECT_MAP — Landing Page Psicóloga Amanda Rodrigues

## Estrutura de arquivos

```
SitePsicologia/
  index.html          ← arquivo principal (HTML + CSS inline, ~736 linhas)
  corporativo.html    ← página para público corporativo
  CNAME               ← domínio GitHub Pages
  README              ← descrição do repositório
  CLAUDE.md           ← instruções para Claude Code
  PROJECT_MAP.md      ← este arquivo
  .claude/
    agents/           ← agentes Claude Code
      psychology-expert.md
      seo-specialist.md
      copywriter.md
      frontend-dev.md
      qa-reviewer.md
    settings.json
    settings.local.json
  .github/
    copilot-instructions.md   ← instruções para DeepSeek/Copilot
    prompts/                  ← skills Copilot (equivalentes aos agents)
      psychology-expert.prompt.md
      seo-specialist.prompt.md
      copywriter.prompt.md
      frontend-dev.prompt.md
      qa-reviewer.prompt.md
  .vscode/
    settings.json             ← configurações do workspace VS Code
```

## Estrutura do index.html

### Variáveis CSS (`:root`)
```
--lilac, --lilac-light, --lilac-deep   cores lilás
--cream                                 fundo principal
--rose, --rose-light, --rose-pale       tons rose/blush
--text, --text-light                    tipografia
--white, --blush                        auxiliares
```

### Fontes
- `Playfair Display` — headings (serifada, elegante)
- `Lato` — corpo do texto (sans-serif, legível)

### Seções da página (em ordem)

| Seção | Descrição |
|---|---|
| `<header>` / nav | Logo + navegação com links âncora |
| Hero | Headline principal, subtítulo, CTA primário |
| Sobre | Bio da psicóloga, formação, abordagem |
| Serviços | Cards com os tipos de atendimento |
| Para quem | Identificação do público-alvo |
| Como funciona | Passos do processo de atendimento |
| Depoimentos | Prova social |
| FAQ | Perguntas frequentes |
| Contato / CTA final | Formulário ou botão WhatsApp |
| `<footer>` | Links, redes sociais, CRP |

## Decisões técnicas conhecidas

- CSS 100% inline no `<style>` — sem arquivo externo
- Sem JavaScript (página estática)
- Hospedagem via GitHub Pages (CNAME configurado)
- Fontes carregadas via Google Fonts CDN
