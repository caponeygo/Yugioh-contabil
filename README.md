# Yugioh Contábil

Flashcards para o Exame de Suficiência CFC 2026. Site estático, sem build. Progresso salvo no `localStorage`; login e ranking via Supabase.

## Volumes (`questoes/*.json`)
- `exame-2026-2.json`: prova real 2026.2, Tipo 1 (50 questões)
- `exame-2026-1.json`: prova real 2026.1, Tipo 2 (50 questões)
- `vol-3.json`: 48 questões autorais

**Atenção:** as provas reais não trazem gabarito. As respostas e explicações foram resolvidas por IA e não são o gabarito oficial da FGV. Confira antes de confiar.

Para adicionar um volume: crie `questoes/<id>.json` (lista de `{d, q, o, e}`, com a alternativa correta em `o[0]`) e inclua o `id` em `VOLS` no `index.html`.

Veja [RESUMO.md](RESUMO.md).
