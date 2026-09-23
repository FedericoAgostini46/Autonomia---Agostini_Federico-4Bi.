# Esercizio 3 — Tre tipi di apprendimento

1. **Un sistema che raggruppa gli articoli di un quotidiano per argomento senza che gli argomenti siano stati definiti in anticipo**
   * **Tipo di apprendimento:** Non supervisionato.
   * **Motivazione:** Le etichette sono **assenti**; il sistema deve identificare autonomamente le strutture sottostanti e i gruppi (clustering) senza guida preventiva.

2. **Un programma che impara a parcheggiare un'automobile in un simulatore ricevendo un punteggio a ogni tentativo**
   * **Tipo di apprendimento:** Per rinforzo.
   * **Motivazione:** Le etichette sono **sostituite da un segnale di premio** (punteggio), che la macchina usa per imparare la sequenza di azioni ottimali per prova ed errore.

3. **Un sistema che riconosce la specie di un pinguino addestrato sulle 344 osservazioni dell'arcipelago Palmer;**
   * **Tipo di apprendimento:** Supervisionato.
   * **Motivazione:** Le etichette sono **presenti** nel dataset di addestramento (la colonna `species` per ciascuna riga).

4. **Un sistema che segnala le transazioni bancarie insolite senza disporre di un elenco di frodi già accertate;**
   * **Tipo di apprendimento:** Non supervisionato.
   * **Motivazione:** Le etichette sono **assenti**; il sistema individua le anomalie rilevando gli scostamenti dai modelli di comportamento standard del dataset.

5. **Un sistema che stima il tempo di percorrenza di un tragitto a partire dallo storico dei tragitti già compiuti e cronometrati.**
   * **Tipo di apprendimento:** Supervisionato.
   * **Motivazione:** Le etichette sono **presenti**, rappresentate dai tempi effettivi cronometrati e registrati per ogni tragitto storico.