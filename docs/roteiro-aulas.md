# Roteiro de aula

Progressão pensada para ser mostrada ao vivo, sem precisar de slides
teóricos longos — o próprio `demo-site/` vai contando a história.

> Este repositório já tem `CLAUDE.md`/`AGENTS.md` e `.claude/` reais na
> raiz (é assim que ele deve ficar para quem for clonar e usar depois da
> aula). Para os Blocos 1 e 2 funcionarem como demonstração "do zero",
> esconda o contexto real antes de começar e restaure o `demo-site/`
> entre uma rodada e outra usando o próprio git (o repositório já está
> versionado, então isso é instantâneo e não exige sair da pasta):
>
> ```bash
> # antes dos blocos 1 e 2: esconder o contexto real
> mv CLAUDE.md CLAUDE.md.bak
> mv AGENTS.md AGENTS.md.bak
>
> # depois de cada rodada, para voltar demo-site/ ao estado original
> git restore demo-site/
> git clean -fd demo-site/
>
> # ao entrar no bloco 3: devolver o contexto
> mv CLAUDE.md.bak CLAUDE.md
> mv AGENTS.md.bak AGENTS.md
> ```

## Bloco 1 — Prompt mínimo → o que fazer

Com `CLAUDE.md`/`AGENTS.md` escondidos, rodar o prompt de
`prompt-experiments/01-prompt-minimo.md` contra `demo-site/`. Observar e
anotar as decisões que o agente tomou sozinho.

## Bloco 2 — Prompt estruturado → como fazer, o que não fazer, critério de pronto

Rodar `git restore demo-site/ && git clean -fd demo-site/` para desfazer
o Bloco 1, depois o prompt de `prompt-experiments/02-prompt-estruturado.md`.
Preencher `prompt-experiments/comparacao.md` junto com a turma.

## Bloco 3 — AGENTS.md / CLAUDE.md → regras permanentes do projeto

Desfazer o Bloco 2 (`git restore demo-site/ && git clean -fd demo-site/`)
e devolver `CLAUDE.md`/`AGENTS.md` aos seus nomes originais. Rodar de
novo o prompt mínimo do Bloco 1 e mostrar que, mesmo curto, o resultado
se aproxima do Bloco 2 — porque as regras já estão no contexto do
projeto automaticamente.

## Bloco 4 — Skill de revisão → procedimento reutilizável

Ainda na raiz do repositório (onde `.claude/skills/frontend-review/` e
`.claude/agents/revisor.md` já existem), pedir "revise a implementação
do dark mode" ou acionar o subagente `revisor` diretamente. Mostrar a
skill/subagente sendo acionado como procedimento reutilizável, em vez de
reescrever a checklist toda vez no prompt.

## Bloco 5 — Desafio final → aluno pratica sozinho

Aluno repete o processo completo (prompt mínimo → observação → prompt
estruturado → comparação) sobre a tarefa descrita em `desafio-final/`.

## Plano B — e se o Bloco 1 sair certo de primeira?

Pode acontecer, principalmente com modelos mais cuidadosos. Não é um
problema para a aula, é o próprio ponto seguinte:

> "E se ele acertar de primeira? Ótimo — é exatamente o argumento: um
> modelo moderno consegue salvar um prompt ruim. Só que você não pode
> contar com isso em produção, porque o resultado não é determinístico.
> A mesma pergunta, rodada de novo, pode sair diferente."

Ensaiem o Bloco 1 na noite anterior, com a ferramenta que será usada em
aula, e guardem um print/diff do resultado como backup — mesmo que o
resultado "funcione", quase sempre há pelo menos uma decisão que o
agente tomou sozinho (onde ficou o botão, se usou `localStorage`, se
reaproveitou as CSS variables ou sobrescreveu cores direto no
componente) que vale a pena apontar ao vivo.
