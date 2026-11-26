---
repo: obi2kenobi
linguaggi: nessuno (solo documentazione)
stato: documentazione iniziale, nessun codice
aggiornato: 2026-11-26
---

# Scheda tecnica — obi2kenobi

## Scopo
Repository in fase iniziale: nessun codice, nessun entry point, nessun dipendente. La documentazione è l'unico artefatto.

## Architettura
Documentazione-only. Branch docs/g7-giro5-2026-11 (worktree, non checkout principale). Nessun layout di codice.

## Componenti
| Nome | Ruolo | File |
|------|-------|------|
| README.md | stato reale del repo | README.md |
| docs/LLM-GUIDA.md | guida LLM onesta | docs/LLM-GUIDA.md |
| docs/ISTRUZIONI.md | istruzioni d'uso | docs/ISTRUZIONI.md |
| docs/CLAUDE.md | contesto per agenti | CLAUDE.md |
| Artefatti di revisione | processi M-017.3, non guida | docs/_inventario.tsv, docs/_guida-lista.txt, docs/_revisione.tsv |

## Dati e interfacce
Nessuna. Nessun dato, storage o interfaccia.

## Dipendenze
Nessuna. Nessun file di dipendenze (package.json, requirements.txt, pyproject.toml, go.mod) presente.

## Configurazione
Nessuna variabile d'ambiente documentata. Segreti: nessuno; non committare valori reali.

## Build e test
Non verificato: nessun comando di installazione/build/test reale. Verifica: `git log --oneline -1` e `git status --short`.

## Deploy
Non disponibile: nessun codice da deployare.

## Rischi e debito tecnico
- Repo senza codice: qualsiasi doc che elenchi comandi reali sarebbe falso.
- Artefatti di processo non sono guida.
- README/LLM-GUIDA possono risultare stale: aggiornare quando il codice apparirà.
