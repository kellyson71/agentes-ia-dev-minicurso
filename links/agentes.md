# Agentes, AGENTS.md, CLAUDE.md e Skills — documentação oficial

Os três links de destaque para a aula (fecham o "ecossistema de agentes"
sem virar uma aula infinita de prompt engineering):

1. **OpenAI:** `AGENTS.md` + Skills + prompts —
   [Rethinking Skills and Prompts for GPT-6 Astra](https://developers.openai.com/blog/rethinking-skills-and-prompts-for-gpt-6-astra)
   (leitura obrigatória: resume exatamente o assunto do minicurso).
2. **Anthropic:** `CLAUDE.md` + Skills + Agents + Hooks —
   [Steering Claude Code](https://claude.com/blog/steering-claude-code-skills-hooks-rules-subagents-and-more)
   (melhor material para explicar a diferença entre essas peças).
3. **Google:** Antigravity criando → desenvolvendo → implantando uma app —
   [Build and Deploy to Google Cloud with Antigravity](https://codelabs.developers.google.com/build-and-deploy-gcp-with-antigravity)
   (codelab prático, também [em português](https://codelabs.developers.google.com/build-and-deploy-gcp-with-antigravity?hl=pt-br)).

## OpenAI / Codex

- [Skills — OpenAI Developers](https://developers.openai.com/api/docs/guides/tools-skills) —
  estrutura de `SKILL.md`, instruções reutilizáveis e arquivos auxiliares.
- [Usar Skills para acelerar manutenção de OSS](https://developers.openai.com/blog/skills-agents-sdk) —
  caso real: equipe do OpenAI Agents SDK usa `AGENTS.md` + Skills + GitHub
  Actions para automatizar tarefas repetitivas.
- [Testando Skills sistematicamente com avaliações](https://developers.openai.com/blog/eval-skills) —
  não basta criar uma Skill, é preciso avaliar se ela funciona de fato.
- [OpenAI Agents SDK — exemplo de AGENTS.md](https://github.com/openai/openai-agents-python/blob/main/AGENTS.md) —
  projeto real usando `AGENTS.md`, bom para abrir ao vivo na aula.

## Claude Code

- [Claude Code — skill de estrutura de plugins/Skills](https://github.com/anthropics/claude-code/blob/main/plugins/plugin-dev/skills/plugin-structure/SKILL.md) —
  exemplos concretos de estrutura de `skills/`, `agents/`, comandos.
- [Claude Code — desenvolvimento de Agents](https://github.com/anthropics/claude-code/blob/main/plugins/plugin-dev/skills/agent-development/SKILL.md) —
  como um Agent define descrição, ferramentas permitidas e gatilhos.
- [Exemplos completos de Agents do Claude Code](https://github.com/anthropics/claude-code/blob/main/plugins/plugin-dev/skills/agent-development/examples/complete-agent-examples.md) —
  inclui um `code-reviewer` pronto como referência.

## Gemini / Antigravity

- [Google Codelab — Criando Agent Skills para Gemini CLI](https://codelabs.developers.google.com/gemini-cli/how-to-create-agent-skills-for-gemini-cli) —
  mostra a criação de uma pasta com `SKILL.md` e como o Gemini CLI a usa
  (também [em português](https://codelabs.developers.google.com/gemini-cli/how-to-create-agent-skills-for-gemini-cli?hl=pt-br)).
