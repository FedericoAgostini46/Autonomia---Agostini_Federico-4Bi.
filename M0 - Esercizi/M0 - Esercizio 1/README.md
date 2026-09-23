# Esercizio 1 — Riconoscere istanze, attributi ed etichetta

## 1. Conteggio Istanze e Attributi
* **Numero di istanze (righe):** 344
* **Numero di attributi (colonne):** 7
* **Nomi esatti delle colonne:**
  1. `species`
  2. `island`
  3. `bill_length_mm`
  4. `bill_depth_mm`
  5. `flipper_length_mm`
  6. `body_mass_g`
  7. `sex`

---

## 2. Domande

### Domanda A: *«A quale specie appartiene un pinguino di cui conosco le misure?»*
* **Etichetta (Target / Output):** `species`
* **Colonne in ingresso (Features / Input):** `bill_length_mm`, `bill_depth_mm`, `flipper_length_mm`, `body_mass_g`.

### Domanda B: *«Quanto pesa un pinguino di cui conosco specie, isola e misure del becco?»*
* **Etichetta (Target / Output):** `body_mass_g`
* **Colonne in ingresso (Features / Input):** `species`, `island`, `bill_length_mm`, `bill_depth_mm`.

---

## 3. Conclusione
L'etichetta cambia perché non è una proprietà intrinseca o fissa del dataset, ma dipende dal problema di apprendimento che si sceglie di risolvere e dalla variabile che si desidera prevedere.
Il dataset contiene i dati grezzi raccolti; è l'obiettivo dell'analisi stabilire quale colonna faccia da output target e quali da dati di input.