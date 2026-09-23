# Agentes de IA para Desenvolvimento — Minicurso

Este repositório é material de apoio para um minicurso prático sobre
agentes de IA aplicados a desenvolvimento de software. A peça central é
`demo-site/`, uma landing page simples usada para demonstrar, ao vivo, a
diferença entre um prompt mínimo e um prompt estruturado.

## Regras do projeto

- Preserve a estrutura existente de `demo-site/`.
- Prefira reutilizar as CSS variables definidas em `:root` (em
  `demo-site/style.css`) ao invés de sobrescrever cores diretamente nos
  componentes.
- Não adicione dependências, frameworks ou build steps sem necessidade —
  `demo-site/` deve continuar rodando apenas abrindo `index.html`.
- Não altere conteúdo (textos, seções) sem solicitação explícita.
- Mantenha o layout responsivo.

## Skills e subagentes disponíveis

- Skill `frontend-review` (`.claude/skills/frontend-review/`): revisão de
  alterações de UI sem aplicar correções automaticamente.
- Subagente `revisor` (`.claude/agents/revisor.md`): confere se uma
  alteração recente respeita as regras acima.
- Subagente `documentador` (`.claude/agents/documentador.md`): mantém
  `README.md` e `docs/roteiro-aulas.md` sincronizados com a estrutura real
  do repositório.

## Estrutura

- `demo-site/` — projeto de demonstração (HTML/CSS/JS puro).
- `prompt-experiments/` — prompts e anotações dos experimentos de dark
  mode (mínimo vs. estruturado).
- `desafio-final/` — segunda tarefa para prática livre.
- `docs/roteiro-aulas.md` — roteiro de aula em 5 blocos.
- `ACOMPANHAMENTO.md` — links e materiais de apoio da preparação do curso.
- `slides-agentes-ia-dev.pdf` — slide completo da aula.

Veja `docs/roteiro-aulas.md` para a sequência pedagógica completa.
