# GateTimer

Cronometro per **sprint** e **navetta** che usa la webcam come fotocellula virtuale: due linee sullo schermo rilevano il passaggio dell'atleta e avviano/fermano il tempo.

**Apri l'app:** https://enzocaravano-gk.github.io/gatetimer/

## Come si usa
1. Apri il link da tablet, telefono o computer e consenti l'accesso alla camera.
2. Metti il dispositivo su un cavalletto, di lato rispetto alla corsia.
3. Trascina le linee sui punti di partenza e arrivo (in navetta: START/FINE e CONO).
4. Regola la sensibilità se il timer scatta da solo o non scatta.

## Funzioni
- **Sprint:** START → END.
- **Navetta:** START → CONO (tempo di andata) → ritorno su START.
- Tempo interpolato tra i fotogrammi, con contatore fps visibile.
- Bip sonori e vibrazione a ogni passaggio (🔊 nell'intestazione).
- Tema chiaro ad alto contrasto per l'uso all'aperto (☀️ nell'intestazione).
- Sessioni con nome, report PDF con anteprima e storico delle sessioni.
- Anagrafica atleti e squadre, importazione da Excel/CSV.

I dati restano solo sul dispositivo su cui vengono registrati (memoria del browser).

## Sviluppo
È un unico file, `index.html`, senza passaggi di build. Per provarlo in locale serve un server (la camera richiede `localhost` o `https`):

```bash
python3 -m http.server 8765
```

poi apri http://localhost:8765.
