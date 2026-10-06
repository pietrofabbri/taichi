# Analisi strutturale iniziale — pietrofabbri/taichi

Data analisi: 2026-10-06
Fonte: clone locale di `pietrofabbri/taichi`, branch `master`, commit `191bed5` ("Prima stesura del corso...")

## 1. Che cos'è questo repo

È un **corso di studio personale in italiano** sul Tai Chi Chuan (stile Yang), uscito da una singola prima stesura. Non è un wiki, non è un sito, non è un corso pubblico strutturato in piattaforma. È sequenziale, testuale, auto-riferito, con una progressione didattica esplicita dalla teoria alle pratiche propedeutiche fino alla Forma 24.

Nota importante: il materiale video/audio/PDF di partenza non è incluso per diritti d'autore. Il repo contiene solo contenuti originali o di dominio pubblico/fonti aperte, citate.

## 2. Stato del repo

- Branch: `master`
- Commit visibile: un solo commit iniziale
- Remote: `origin https://github.com/pietrofabbri/taichi.git`
- File dirottati nel repo: README.md, .gitignore, più 20 file di contenuto Markdown

INTERPRETAZIONE: a prima vista il repo è compatibile con un "mono-commit iniziale" piuttosto che con un progetto in evoluzione documentato nel tempo. Tuttavia, non posso escludere che ci siano commit successivi non ancora visibili in questa scansione. Da verificare con un log più ampio se serve.

## 3. Struttura dei contenuti

### 3.1 Organizzazione per moduli

- `00-fondamenta/` — basi concettuali e corporee
- `01-qigong/` — pratiche propedeutiche
- `02-medicina-tradizionale-cinese/` — quadro teorico MTC
- `03-storia-e-stili/` — contesto storico e stili
- `04-forma-24/` — la forma frammentata in 4 sezioni + overview
- `05-risorse/` — fonti e bibliografia

Questa struttura rispecchia esattamente l'ordine didattico proposto nel README.

### 3.2 Contenuti per fascia

Fondamenta:
- principi taoisti e Taiji
- postura e allineamento
- respirazione
- radicamento ed equilibrio
- camminata Tai Chi

Qi Gong:
- introduzione
- Zhan Zhuang
- Baduanjin

MTC:
- Qi
- Yin/Yang
- Wu Xing
- meridiani e organi Zang-Fu
- rapporto Tai Chi–MTC e le 8 energie

Storia e stili:
- origine leggenda
- principali stili

Forma 24:
- overview con sequenza completa
- 4 sezioni da 6 movimenti

Risorse:
- fonti

## 4. Qualità e stile dei contenuti (campione)

Da quanto letto, il repo:

- mantiene un italiano Chiaro;
- cita spesso i file interni come riferimenti incrociati;
- integra concetti teorici con applicazioni pratiche alla forma;
- separa esplicitamente teoria da avvertenze pratiche (es. la nota metodologica in fonti.md e il disclaimer sul video);
- cita fonti web di dominio pubblico:
  - Wikipedia (24-form tai chi, Baduanjin, Zhan zhuang, TCM)
  - Qialance per nomi dei movimenti

CERTO: il livello di precisione sembra adeguato a un corso di studio personale, non a un testo di riferimento accademico o a un manuale federativo.

## 5. Punti di forza

- Progressione didattica chiara e autoconsistente.
- Cross-referenziazione interna molto fitta tra moduli.
- Distinzione conservata tra cosa è teoria, cosa è pratica, cosa è riferimento video.
- Forma 24 mappata con nome cinese, pinyin, italiano e sezione.

## 6. Incompletezze visibili

Da README:

- applicazioni marziali movimento per movimento sono segnate come incompiute;
- integrazione con trascrizioni dai video personali non ancora fatta;
- note di pratica/log del progresso ancora assenti.

INTERPRETAZIONE: il repo è probabilmente legato alla pratica personale del proprietario e pensato per essere espanso con l'esperienza.

Da campione di lettura:

- le sezioni teoriche sono complete in sé, ma alcune sono dense e presuppongono la lettura incrociata.
- non ho ancora verificato se tutti i collegamenti interni puntano a file effettivamente esistenti.

## 7. Possibili obiettivi del repo AI

(Il repo AI non dovrebbe sostituire il repo di produzione, ma può supportarlo.)

Idee possibili:

- mappe concettuali dei nodi teorici (Wuji/Taiji, Yin-Yang, Wu Xing, Ba Jin, postures, respiro);
- scheda di studio per movimento della Forma 24;
- tabella di coerenza tra principi fondamentali e movimenti);
- inventario dei collegamenti interni reali vs. citazioni presenti nel testo;
- confronto tra le definizioni del repo e le fonti web citate (es. Wikipedia e Qialance);
- glossario cinese/italiano/pinyin;
- report su incompletezze e prossimi passi;
- evidenziazione di contraddizioni o passaggi poco chiari.

Queste sono suggerimenti, non decisioni. La direzione va stabiliizzata con l'utente.

## 8. Limiti di questa analisi

- Non ho potuto clonare `pietrofabbri/taichi-ai`, quindi il repo AI è stato creato localmente qui e rimane un laboratorio manuale.
- Ho letto solo un sottoinsieme dei file: il report è basato su un campione rappresentativo, non su una verifica file per file completa.
- Non ho verificato i link esterni in modo attivo, né il rispetto delle citazioni rispetto alle fonti.
- L'affermazione "un solo commit" è basata su `git log -n 20`; può essere incompleta se il repo ha storia più articolata.

## 9. Prossimi passi possibili

Nota di verifica immediata: nel campione controllato ho trovato due incoerenze di collegamento interno da verificare/correggere nel repo di produzione (non modificate qui automaticamente):

- `00-fondamenta/04-radicamento-ed-equilibrio.md` cita `06-camminata-tai-chi.md` (riga 19, link interno), ma il file presente è `05-camminata-tai-chi.md`.
- `01-qigong/01-introduzione-qigong.md` cita `02-zhan-zhuang.md` e `03-baduanjin-otto-pezzi-di-broccato.md` con percorsi abbreviati rispetto alla posizione reale dei file.

INTERPRETAZIONE: sembrano errori di digitazione nei riferimenti interni, non mancanze di contenuto, ma vanno corretti se il repo deve restare navigabile in modo coerente.

1. Verifica incrociata completa: ogni riferimento interno esiste nel filesystem?
2. Confronto fonti: Wikipedia/ Qialance vs definizioni del repo per alcuni punti chiave.
3. Scheda Forma 24 per movimento: tabelle pronte per studio.
4. Mappa concettuale: nodi e relazioni tra moduli.
5. Definizione con l'utente dello scopo esatto del repo AI.

