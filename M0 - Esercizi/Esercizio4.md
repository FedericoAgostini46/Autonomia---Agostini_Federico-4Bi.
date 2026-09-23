# Esercizio 4 - Scrivere la regola a mano e misurarne gli errori

## 1. Struttura del Foglio e Formula
Per eseguire l'esercizio in Fogli Google (o Microsoft Excel):
1. Si filtrano i dati mantenendo unicamente le righe corrispondenti alle specie **Adelie** e **Gentoo** (totale **276 istanze**, di cui 2 con dati mancanti, per un totale di 274 istanze analizzabili).
2. Nella colonna `H` (chiamata `Previsione`) viene inserita la formula condizionale:
   ```excel
   =SE(E(C2 > X; F2 > Y); "Gentoo"; "Adelie")


## 2. Registro dei Tentativi e Risultati
| Tentativo | Soglia Pinna ($X$) | Soglia Massa ($Y$) | Formula applicata | Conteggio Errori | % Errore |
| :---: | :---: | :---: | :--- | :---: | :---: |
| **Tentativo 1** | $> 205\text{ mm}$ | $> 4700\text{ g}$ | `=SE(E(C2>205; F2>4700); "Gentoo"; "Adelie")` | **33** / 274 | 12.04% |
| **Tentativo 2** | $> 200\text{ mm}$ | $> 4500\text{ g}$ | `=SE(E(C2>200; F2>4500); "Gentoo"; "Adelie")` | **18** / 274 | 6.57% |
| **Tentativo 3** | $> 198\text{ mm}$ | $> 4200\text{ g}$ | `=SE(E(C2>198; F2>4200); "Gentoo"; "Adelie")` | **10** / 274 | 3.65% |


## 3. Domanda
### Domanda: *«che cosa hai fatto, in questo esercizio, che nel corso verrà fatto da una procedura automatica, e che cosa hai dovuto decidere tu?»*

In questo esercizio ho fatto a mano quello che di solito fa un programma di Intelligenza Artificiale.

Cosa ho fatto io a mano, che in futuro farà il computer in automatico:
- Guardare i dati e cercare il limite giusto: Ho osservato la lunghezza delle pinne e il peso dei pinguini, provando a occhio a capire da dove i pinguini Gentoo iniziano a essere diversi dagli Adelie.
- Provare e correggere gli errori: Ho cambiato più volte i numeri limite (le soglie) per fare meno errori possibili, passando da 33 errori a soli 10. Il computer fa la stessa identica cosa: prova da solo tantissime combinazioni matematiche finché non trova i numeri perfetti per sbagliare il meno possibile.

Cosa ho dovuto decidere io di mia testa (e che deve sempre decidere l'uomo):
- Quali dati usare: Ho scelto io di guardare solo la lunghezza della pinna e il peso, tralasciando le altre informazioni del file.
- Come creare la regola: Ho deciso io la forma del ragionamento (usare la regola del "SE la pinna è più lunga di X E il peso è maggiore di Y").
- Quando accontentarmi: Ho deciso io quando fermarmi con i tentativi, ritenendo che fare solo 10 errori fosse un risultato sufficientemente buono.