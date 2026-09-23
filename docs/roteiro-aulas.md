# Roteiro de aula

Progressão pensada para ser mostrada ao vivo, sem precisar de slides
teóricos longos — o próprio `demo-site/` vai contando a história.

> Este repositório já tem `CLAUDE.md`/`AGENTS.md` e `.claude/` reais na
> raiz (é assim que ele deve ficar para quem for clonar e usar depois da
> aula). Para os Blocos 1 e 2 funcionarem como demonstração "do zero",
> rode o agente **numa cópia isolada de `demo-site/`, fora do
> repositório**, para que nenhum `CLAUDE.md`/`AGENTS.md` seja lido:
>
> ```bash
> cp -r demo-site /tmp/demo-bloco1
> cd /tmp/demo-bloco1
> ```

## Bloco 1 — Prompt mínimo → o que fazer

Dentro de `/tmp/demo-bloco1` (sem nenhum `CLAUDE.md`/`AGENTS.md` no
caminho), rodar o prompt de `prompt-experiments/01-prompt-minimo.md`.
Observar e anotar as decisões que o agente tomou sozinho.

## Bloco 2 — Prompt estruturado → como fazer, o que não fazer, critério de pronto

Repetir com uma cópia nova (`cp -r demo-site /tmp/demo-bloco2`) e o
prompt de `prompt-experiments/02-prompt-estruturado.md`. Preencher
`prompt-experiments/comparacao.md` junto com a turma.

## Bloco 3 — AGENTS.md / CLAUDE.md → regras permanentes do projeto

Voltar para a raiz do repositório de verdade (onde `CLAUDE.md`/
`AGENTS.md` já existem). Rodar de novo o prompt mínimo do Bloco 1,
agora contra `demo-site/` dentro do repositório, e mostrar que, mesmo
curto, o resultado se aproxima do Bloco 2 — porque as regras já estão no
contexto do projeto automaticamente.

## Bloco 4 — Skill de revisão → procedimento reutilizável

Ainda na raiz do repositório (onde `.claude/skills/frontend-review/` e
`.claude/agents/revisor.md` já existem), pedir "revise a implementação
do dark mode" ou acionar o subagente `revisor` diretamente. Mostrar a
skill/subagente sendo acionado como procedimento reutilizável, em vez de
reescrever a checklist toda vez no prompt.

## Bloco 5 — Desafio final → aluno pratica sozinho

Aluno repete o processo completo (prompt mínimo → observação → prompt
estruturado → comparação) sobre a tarefa descrita em `desafio-final/`.
