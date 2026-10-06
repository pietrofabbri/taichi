# TASK 001 — Verifica collegamenti interni del repo di produzione

## Ruolo

Laguna = operatore tecnico / elaboratore.

Solar = autore del task e verificatore del risultato.

## Obiettivo

Scoprire tutti i collegamenti interni ai file Markdown del repo di produzione e segnalare quali sono probabilmente rotti o ambigui.

Non modificare il repo di produzione.

## Input

- `../../taichi` — clone locale di `pietrofabbri/taichi`
- ambito: tutti i file `*.md` sotto `taichi/`, esclusi `.git`

## Output

`.ai/HANDOFF/TO-SOLAR/result-001-verifica-collegamenti-interni.md`

## Formato

Il risultato deve essere un report Markdown con:

1. Metodo usato
2. Ambito esatto ispezionato
3. Lista dei link interni trovati, uno per riga, con:
   - file sorgente
   - link citato
   - tipo di aspettativa (es. file locale Markdown, percorso relativo)
4. Lista dei link con problema rilevato
5. Per ogni problema:
   - descrizione
   - file sorgente
   - link citato
   - cosa esiste effettivamente nel filesystem, se disponibile
6. Nota sui casi ambigui
7. Limiti del report

## Regole operative

- Raccogliere i link dai file Markdown con uno strumento automatico compatibile con ripgrep/relpath, non a mano.
- Un link interno è probabile riferimento a un file locale quando:
  - punta a un percorso relativo che sembra un file Markdown
  - o punta a un percorso che, nel contesto del repo, sembra riferirsi a un file del repo
- Non raddrizzare i link nel repo di produzione.
- Non inventare corrispondenze: se un link non è chiaramente un riferimento file, marcalo come ambiguo.
- Distinguere chiaramente tra:
  - link assente nel filesystem
  - link a nome file diverso da quello effettivo
  - link ambiguo o non verificabile con questo metodo

## Cosa non deve essere modificato

- `../../taichi`
- nessun file del repo di produzione

## Fonti da usare

- solo contenuto dei file Markdown nel repo di produzione
- solo struttura file effettiva nel clone locale

## Livello di autonomia

- procedura eseguita in modo meccanico
- interpretazione dei casi dubbi: segnalarli, non decidere al posto di Solar

## Verifiche richieste nel risultato

Il risultato deve permettere a Solar di:

- ripetere il metodo in suite
- capire quali link sono stati considerati OK e perché
- capire quali sono stati segnalati e perché
- distinguere segnala da interpretazione

## Stato

READY
