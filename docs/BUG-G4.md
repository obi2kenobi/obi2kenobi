# BUG-G4 — candidati bug (M-031.51b.1)

CANDIDATO-1: docs/LLM-GUIDA.md:5 — afferma "README.md — stato reale del repo (23 righe)" ma `wc -l README.md` = 24; inventario.tsv riporta anche "LLM-GUIDA.md 25" contro le 31 righe reali: dati inconsistenti/falsi nella guida.
CANDIDATO-2: CLAUDE.md:7 e docs/LLM-GUIDA.md:8 — affermano "Commit: f407590" / "f407590 (2026-11-24)" mentre git log mostra HEAD = 9299301/fa960b8; documentazione stale che contraddice il repo reale.
CANDIDATO-3: docs/_revisione.tsv — afferma che le osservazioni "DA CORREGGERE" sul branch/commit sono state registrate ma il ramo reale è fix/g4-2026-11 (worktree) e README dice ancora "docs/g7-giro2-2026-11" — coerenza non verificata.

NON corretto: solo analisi (nessun codice da correggere).
