# Agentes de IA para Desenvolvimento — Minicurso

<img src="assets/logo-minicurso.png" alt="Mini Curso: IA para desenvolvimento, do modelo ao agente" width="100%" />

Material de apoio para um minicurso prático sobre agentes de IA aplicados
a desenvolvimento de software (Claude Code, Codex, Gemini CLI e afins como
exemplos), ministrado na 9ª Expotec do Campus Pau dos Ferros do IFRN
(23 a 25/09/2026).

## Ideia central

Em vez de uma aula teórica sobre agentes, o curso conta essa história
usando um único projeto pequeno (`demo-site/`):

```
Prompt mínimo
    ↓
Prompt estruturado (restrições + critério de pronto)
    ↓
AGENTS.md / CLAUDE.md (regras permanentes do projeto)
    ↓
Skill (procedimento reutilizável)
    ↓
Desafio final (aluno pratica sozinho)
```

O roteiro completo está em [`docs/roteiro-aulas.md`](docs/roteiro-aulas.md).

## Sobre a oficina

- **Evento:** 9ª Expotec — Exposição Científica, Tecnológica e Cultural do
  Campus Pau dos Ferros (IFRN), tema "Ciência Delas: Inspirando Gerações,
  Transformando o Alto Oeste".
- **Data do evento:** 23 a 25/09/2026.
- **Oficina "Agentes de IA para Desenvolvimento":** 24/09/2026, das 07:30
  às 10:30 (3h), Campus Pau dos Ferros.
- **Inscrição no evento:** pelo Suap (participante) ou pela plataforma
  [Even3](https://www.even3.com.br/9-expotec-campus-pau-dos-ferros-ifrn-759082/)
  (submissão de trabalhos).

## Estrutura do repositório

- `demo-site/` — landing page simples usada como terreno de demonstração
  ao vivo (HTML/CSS/JS puro, sem build step — basta abrir `index.html`).
- `prompt-experiments/` — os dois prompts (mínimo e estruturado) usados na
  demonstração de dark mode, com espaço para anotações da turma.
- `CLAUDE.md` / `AGENTS.md` — regras do projeto, lidas automaticamente
  pelo Claude Code, Codex ou Gemini CLI ao rodar na raiz do repositório.
- `.claude/skills/frontend-review/` — skill real de revisão de frontend.
- `.claude/agents/` — subagentes reais (`revisor`, `documentador`).
- `desafio-final/` — segunda tarefa, com decisão de projeto em aberto,
  para o aluno repetir o exercício sozinho.
- `docs/` — roteiro de aula.
- `links/` — links curados por tema (agentes/AGENTS.md/Skills,
  benchmarks, comunidade, ferramentas) para os alunos acessarem depois.
- `ACOMPANHAMENTO.md` — links e materiais de apoio coletados durante a
  preparação do curso.
- `slides-agentes-ia-dev.pdf` — slide completo da aula.
- `assets/` — logos usadas neste README.

## Como rodar

```bash
cd demo-site
# abrir index.html no navegador
```

Para reproduzir os experimentos, aponte seu agente de IA de preferência
para a pasta `demo-site/` e cole o prompt de
`prompt-experiments/01-prompt-minimo.md` ou
`prompt-experiments/02-prompt-estruturado.md`.

Ao clonar este repositório e rodar `claude` (ou `codex`) na raiz, o
`CLAUDE.md`/`AGENTS.md`, a skill `frontend-review` e os subagentes
`revisor`/`documentador` já ficam disponíveis automaticamente — sem
nenhum passo extra de configuração.

---

<img src="assets/logo-expotec.png" alt="9ª Expotec — Campus Pau dos Ferros IFRN" height="90" />
