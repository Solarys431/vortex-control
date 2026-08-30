<div align="center">

<a href="https://solarys431.github.io/vortex-control/"><img src="assets/banner.png" alt="VORTEX Regia — prototipo di regia software" width="100%"></a>

<strong>Italiano</strong> · <a href="README_EN.md">English</a>

🌐 <a href="https://solarys431.github.io/vortex-control/">Landing page</a>

</div>

---

## Cos'è

VORTEX Regia è un **prototipo funzionale** che riunisce in un unico ambiente software switching, mixer audio, tally, replay, grafiche e rundown. Incorpora **NewsIntelligence**, un aggregatore di notizie basato sull'AI che raccoglie le fonti configurate, valuta le notizie e suggerisce la scaletta del TG, oltre a una **regia vocale** per impartire comandi al sistema. Le decisioni finali restano alla regia e alla redazione.

Le immagini **mostrano il prodotto reale con dati dimostrativi**.

![La plancia di regia VORTEX](assets/software-reale/regia.jpg)

---

## Funzioni principali

### NewsIntelligence — dalla notizia alla scaletta
NewsIntelligence raccoglie le fonti configurate, valuta le notizie e suggerisce la **scaletta del telegiornale**, con indicazioni per grafiche e servizi. L'AI suggerisce, la regia e la redazione decidono.

![NewsIntelligence e proposta della scaletta del TG](assets/software-reale/newsintelligence.jpg)

### Regia vocale — parli, la regia esegue
Il regista **parla in cuffia** e il sistema interpreta i comandi. «AIRSPEED 2 in onda», «lower conduttore», «fai la scaletta dalle notizie» — i comandi appaiono trascritti a schermo e vengono tradotti in azioni controllabili dalla regia.

### Audio broadcast
Una console audio a 18 canali dentro il software: HPF, EQ parametrico, gate, compressore, limiter e pan nel motore audio. Bus per uscita, N-1, master, snapshot e monitoraggio loudness LUFS-S stimato. La voce/AI può comandare anche l'audio.

![Console audio broadcast](assets/software-reale/audio.jpg)

### Switcher, DVE e keyer
Bus PGM/PVW, M/E, transizioni con pattern WIPE, DVE e keyer. DVE, replay, clip e grafiche sono **sorgenti** sui bus: si configurano nei pannelli e si controllano dalla regia.

![DVE e keyer](assets/software-reale/dve.jpg)

### Multiview, tally, replay e grafiche
Il monitor di regia con PVW/PGM, l'anteprima delle grafiche e la mini-multiview degli inviati; supporto tally TSL 3.1/5.0 via UDP; replay da file e webcam; grafiche template HTML compositate su PGM/PVW. L'acquisizione DeckLink per il replay è ancora in sviluppo.

<p>
  <img src="assets/software-reale/multiview.jpg" width="49%" alt="Multiview" />
  <img src="assets/software-reale/replay.jpg" width="49%" alt="Replay" />
</p>
<p>
  <img src="assets/software-reale/grafiche.jpg" width="49%" alt="Grafiche" />
  <img src="assets/software-reale/tally.jpg" width="49%" alt="Tally" />
</p>

### Matrice delle uscite
PGM, CLEAN e AUX verso playout, YouTube e REC: uscite differenziate, ciascuna con il proprio audio, gestite dalla matrice.

![Matrice delle uscite](assets/software-reale/matrice.jpg)

### Log e diagnostica
Gli eventi del sistema — comandi, playout, hardware, AI e voce — sono registrati per livello e modulo, con filtri ed esportazione, per aiutare a ricostruire cosa è successo e quando.

![Pannello Log e diagnostica](assets/software-reale/log.jpg)

---

## Come funziona

Architettura **client-server**: il server mantiene lo stato del mixer e integra i moduli di controllo per CasparCG, DeckLink e tally; la GUI è la superficie di controllo in browser e desktop. Il percorso critico è progettato per non dipendere dai servizi AI, ma le integrazioni hardware e il comportamento operativo devono ancora essere validati sul campo. La modalità simulata viene dichiarata nell'interfaccia.

---

## Stato

**Prototipo funzionale, in sviluppo.** Questa repository e la relativa landing sono pubbliche; il codice sorgente dell'applicazione non è incluso. Il sito è statico, senza cookie né tracciamento; le schermate mostrano il prodotto reale con dati dimostrativi.

<div align="center">

© 2026 Daniele Cappello

</div>
