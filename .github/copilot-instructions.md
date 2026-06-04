# Landing Page — Psicóloga Amanda Rodrigues

Projeto: landing page estática de psicóloga especializada em psicologia perinatal.
Arquivo principal: `index.html` (HTML + CSS inline, sem framework).
Stack compatível: Claude Code + DeepSeek (Copilot) — instruções unificadas.

## Especialidades do projeto

- Psicologia perinatal (gestação, pós-parto, maternagem)
- Público: gestantes, mães recentes, mulheres no ciclo gravídico-puerperal
- Paleta: lilás, rose, cream — tom acolhedor e feminino
- Atendimento: online e presencial

## Agentes / Subagents disponíveis

Ao receber uma tarefa relacionada a este projeto, identifique qual agente
especialista deve ser acionado e delegue para ele usando `runSubagent`.

| Tarefa solicitada | Agente |
|---|---|
| Ética, CFP, conteúdo clínico, terminologia perinatal | `psychology-expert` |
| SEO, meta tags, schema markup, palavras-chave, headings | `seo-specialist` |
| Textos, CTAs, hero section, tom de voz, marketing | `copywriter` |
| HTML semântico, CSS, acessibilidade, responsividade | `frontend-dev` |
| Revisão ampla, auditoria geral, múltiplos aspectos | `qa-reviewer` |

## Regra de roteamento

- Tarefa **específica e clara** → acionar o agente especialista diretamente
- Tarefa **ampla ou com múltiplos aspectos** → acionar `qa-reviewer`
- Nunca acionar mais de 2 agentes para a mesma tarefa
- `qa-reviewer` cobre tudo — não combine com outros

## Restrição global

Todo conteúdo gerado deve respeitar a Resolução CFP nº 6/2019:
sem promessas de resultado, sem urgência manipuladora, sem sensacionalismo.

## Otimização de tokens (DeepSeek / Copilot)

- Sempre leia `PROJECT_MAP.md` ao iniciar uma sessão para contexto estrutural
- Use `semantic_search` antes de `grep_search` para buscas contextuais
- Prefira leituras amplas de arquivo (intervalos grandes) a múltiplas leituras pequenas
- Consulte `/memories/repo/` para fatos já verificados do projeto antes de reanalisar
- Skills em `.github/prompts/` contêm conhecimento detalhado por domínio — carregue sob demanda

## Referência do projeto

Veja `PROJECT_MAP.md` para estrutura detalhada do `index.html`.
