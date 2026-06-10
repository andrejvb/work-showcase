# work-showcase

Anotações **TIL (Today I Learned)** — aprendizados técnicos reais, curtos e datados.

Cada commit aqui é 1 aprendizado genuíno (não green-square farming): 2-3 linhas sobre
algo concreto que aprendi enquanto trabalhava.

- **[CONTRIBUTIONS.md](CONTRIBUTIONS.md)** — índice cronológico, 1 linha por TIL.
- **[til/](til/)** — os arquivos, um por aprendizado (`AAAA-MM-DD-titulo.md`).
- **[bin/showcase](bin/showcase)** — script que captura um TIL, valida o conteúdo e
  faz commit + push automaticamente.

## Como usar

```bash
showcase                       # pergunta o título e abre o editor
showcase "useMemo vs useCallback"
```

O fluxo é "revisão antes": o script abre um rascunho no `$EDITOR`; se eu salvar com
conteúdo real, ele adiciona a linha no índice e commita. Se eu sair vazio, aborta.

Um `post-commit` global (em `~/.git-hooks`) me lembra de rodar `showcase` depois de
qualquer commit nos meus repos de trabalho — sem nunca expor código ou dados da empresa.
