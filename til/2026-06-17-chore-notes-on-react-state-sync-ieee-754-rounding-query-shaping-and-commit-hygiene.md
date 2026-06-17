- Fixing "stale until reload" bugs by recomputing/invalidating derived client state
- Keeping recompute logic consistent across single vs. batch operations
- Rounding floating-point output at the boundary to avoid ...0000005 artifacts
- Selecting only needed columns and dropping unnecessary fallbacks in queries
- Reviewing diffs against conventions and scoping which tests a change impacts# chore: notes on React state sync, IEEE-754 rounding, query shaping and commit hygiene

**Data:** 2026-06-17
**Tags:** <!-- ex: react, performance -->

<!-- escreva aqui o que você aprendeu. apague esta linha. -->
