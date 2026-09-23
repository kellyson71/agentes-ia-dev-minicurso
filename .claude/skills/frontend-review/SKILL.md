---
name: frontend-review
description: Revisa alterações de frontend (HTML/CSS/JS) procurando problemas de responsividade, acessibilidade e consistência visual com os estilos existentes do projeto. Use depois de qualquer mudança em demo-site/ ou em outro código de UI do repositório.
---

# Frontend Review

Ao revisar uma alteração de frontend, verifique nesta ordem:

1. **Consistência com o design system existente** — a alteração reutiliza
   as CSS variables definidas em `:root` (`--primary`, `--background`,
   `--text`, etc.) ou introduziu cores "soltas" hardcoded?
2. **Responsividade** — o layout quebra em telas pequenas (teste mental
   em ~375px de largura)? Foram usados `grid`/`flex` com `minmax`/`auto-fit`
   ou larguras fixas que não adaptam?
3. **Acessibilidade** — os elementos interativos têm foco visível, os
   botões têm texto ou `aria-label` compreensível, o contraste de texto
   permanece legível em ambos os temas (claro/escuro) quando aplicável?
4. **Escopo** — a alteração ficou restrita ao que foi pedido, ou tocou
   arquivos/trechos fora do escopo da tarefa?

## Regras

- Não altere código automaticamente durante a revisão.
- Reporte cada problema encontrado individualmente, citando arquivo e,
  quando possível, a linha ou seletor CSS envolvido.
- Se nada relevante for encontrado, diga isso explicitamente em vez de
  inventar ressalvas.
