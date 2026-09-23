# Experimento 1 — Prompt mínimo

## Prompt usado

```
Adicione um modo escuro nessa página. Quero um botão no header para
alternar entre claro e escuro, com uma aparência moderna.
```

## O que observar durante a execução ao vivo

- Onde o agente colocou o botão?
- Ele usou `localStorage` para persistir a escolha do usuário?
- Ele reutilizou as CSS variables definidas em `:root` (`--primary`,
  `--background`, `--text`) ou sobrescreveu cores diretamente nos
  componentes (`body { background: #111 }`, etc.)?
- Ele criou um arquivo novo (ex.: `dark-mode.js`) ou alterou os existentes?
- Ele mudou alguma cor "por conta própria" (ex.: trocou o `--primary`)?
- Quantos arquivos ele tocou no total?

## Anotações da turma

_(preencher durante a aula)_

-

## Ensaio prévio (2026-09-23, backup caso a demo ao vivo saia diferente)

Resultado real ao rodar este prompt contra o `demo-site/` limpo (sem
`CLAUDE.md`/`AGENTS.md`):

- Botão foi colocado dentro do `<nav>`, misturado com os links, em vez
  de um elemento isolado do header.
- Não reaproveitou as CSS variables existentes: criou cores novas
  hardcoded (`#121212`, `#1e1e1e`, `#b0b0b0`) em vez de um segundo bloco
  `--background`/`--text`/`--surface` para o tema escuro.
- Não persiste a escolha do usuário — sem `localStorage`, o tema volta
  ao claro a cada reload da página.
- 3 arquivos alterados: `index.html`, `script.js`, `style.css`.
