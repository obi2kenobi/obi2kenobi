# BUG-G4 — correzioni (M-031.51b.2)

## BUG-1
Dove: docs/LLM-GUIDA.md:7, docs/_inventario.tsv (righe README/LLM-GUIDA).
Gravità: bassa (dati di guida inconsistenti con il repo reale).
Prova: prima — `wc -l README.md` = 24, `wc -l docs/LLM-GUIDA.md` = 31, inventario diceva 23/25; guida diceva "23 righe". Dopo — inventario 24/31, guida "24 righe".
Correzione: fb5fda2 "docs: aggiorna righe README/LLM-GUIDA (M-031.51b.2 BUG-1)".
Test: `grep -n '24 righe\|31' docs/LLM-GUIDA.md docs/_inventario.tsv`.

## BUG-2
Dove: README.md:11, CLAUDE.md:6-7, docs/LLM-GUIDA.md:10-11 — commit f407590 / branch docs/g7-giro2-2026-11 stale.
Gravità: bassa (documentazione stale che contraddice il repo reale).
Prova: prima — `git log --oneline` mostra HEAD 1b9fd9b; doc citavano f407590. Dopo — doc citano fix/g4-2026-11 / fb5fda2.
Correzione: 231a79e "docs: aggiorna branch e commit (M-031.51b.2 BUG-2)".
Test: `grep -rn 'f407590\|g7-giro2' README.md CLAUDE.md docs/LLM-GUIDA.md` → nessun esito.

## Non fatto (fuori perimetro)
CANDIDATO-3: docs/_revisione.tsv cita branch/commit superati (f407590). Revisioni passate non sono riscrivibili senza rompere l'audit; lasciato come traccia storica, da decidere al Capo.
