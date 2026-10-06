# Handoff protocol

Questo modello è a due ruoli:

- Solar: analisi, ricerca, sintesi, verifica, decisioni metodologiche.
- Laguna: esecuzione tecnica, trasformazione file, formattazione, controlli automatizzabili.

Di memoria:
- produzione: `pietrofabbri/taichi`
- AI: `pietrofabbri/taichi-ai`

Regola di massima: nessun agente modifica direttamente il repo di produzione.

## Flusso

- Solar scrive i task in `.ai/HANDOFF/TO-LAGUNA/`.
- Laguna scrive risultati e report in `.ai/HANDOFF/TO-SOLAR/`.
- Output operativi destinati all'utente o al repo AI possono finire in `.ai/OUTPUT/`.

## Semantica dei stati

Per ora uso stati testuali semplici:

- `READY` = task definito e pronto per l'operatore
- `IN PROGRESS` = lavoro in corso
- `DONE` = operatore ritiene di aver completato il task
- `BLOCKED` = qualcosa manca o è ambiguo
- `REVIEW` = pronta per verifica da parte di Solar

Solar non accetta `DONE` come sinonimo di corretto. Verifica sempre fonte, formato e coerenza.
