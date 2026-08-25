# PhotoVintageMemory

Fotocamera usa-e-getta virtuale che gira interamente nel browser dello smartphone.
Riporta l'attesa e la disciplina della pellicola in una web app: scegli una
pellicola, carica un rullino da 27 scatti, fotografa senza rivedere nulla.
Le foto compaiono solo quando il rullino è finito — oppure 24 ore dopo, come
una volta dal fotografo.

## Come funziona

1. **Scegli la pellicola** tra quattro look, ognuno con anteprima reale:
   - **Classic** — caldo, contrasto morbido, estetica anni 2000
   - **Mono** — bianco e nero contrastato, grana marcata
   - **Beta** — freddo e sbiadito, estetica VHS / Y2K
   - **Cine** — teal & orange cinematografico, grana fine
2. **Scegli lo sviluppo**: reveal immediato a fine rullino, oppure blocco di 24 ore.
3. **Scatta 27 volte.** Tra uno scatto e l'altro devi avanzare la pellicola.
   Nessuna anteprima, nessun ripensamento.
4. **Sviluppa.** Le foto si rivelano tutte insieme; puoi salvarle sul telefono.

Il look viene applicato al momento dello scatto ed è definitivo:
quello che hai fotografato è quello che resta.

## Caratteristiche

- Un solo file `index.html`, nessuna dipendenza, nessun build step
- Nessun backend: foto e stato restano nel dispositivo (IndexedDB)
- Funziona su Android e iPhone dal browser, senza installare app
- Datestamp opzionale impresso sullo scatto
- Salvataggio foto tramite foglio di condivisione (iOS) o download

## Uso

Apri la pagina pubblicata da Safari (iPhone) o Chrome (Android) e consenti
l'accesso alla fotocamera. È richiesto HTTPS: GitHub Pages lo fornisce
automaticamente.

## Note

- Su iOS, se la pagina non viene aperta per circa 7 giorni, Safari può
  cancellare i dati locali. Salva sul telefono le foto a cui tieni.
- Il blocco di 24 ore usa l'orologio del dispositivo.
- I parametri delle pellicole sono nell'oggetto `FILMS` in cima al file
  e si possono tarare liberamente.

## Licenza

MIT
