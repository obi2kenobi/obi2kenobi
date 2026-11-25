# CLAUDE.md — obi2kenobi

Repo in fase iniziale: nessun codice, nessun dipendente, nessun entry point al 2026-11-24. La documentazione è l'unica artefatto.

## Stato reale (verificato)
- Branch: fix/g4-2026-11 (worktree, non il checkout principale).
- Commit HEAD: fb5fda2 "docs: aggiorna righe README/LLM-GUIDA (M-031.51b.2 BUG-1)" (2026-11-25).
- File tracciati: README.md, docs/LLM-GUIDA.md.
- Artefatti di revisione (non committare come guida): docs/_inventario.tsv, docs/_guida-lista.txt, docs/_revisione.tsv.

## Comandi
- Nessun comando di installazione/avvio/test reale: nessun codice. Non inventare comandi.
- Quando il codice apparirà, aggiungere: installazione, build, avvio, test, riportando l'esito verificato.

## Convenzioni
- Non committare segreti reali. Placeholder tipo ${SEGRETO_DA_INSERIRE} ammessi, valori reali vietati.
- Documentazione onesta: descrivere solo lo stato verificato, mai dettagli inventati.
- Aggiornare README.md e docs/LLM-GUIDA.md quando il codice sarà presente.

## Punti fragili
- Repo senza codice: qualsiasi doc che elenchi comandi reali è falso.
- Artefatti _revisione.tsv/_inventario.tsv/_guida-lista.txt sono artefatti di processo; non sono guida.

## Cosa non toccare
- Nessun push senza autorizzazione (il push lo fa il Capo).
- Non lavorare nel checkout principale; solo nel worktree.
- Non cancellare file. Usarli come snapshot di audit.
