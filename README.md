# Progetto finale di Estrazione e Integrazione della conoscenza dei dati

## Esercizio 1
* **Richiesta**: realizzare una funzione che generi una transazione di lunghezza `days` ogni `stride_days`, e conti quante delle transazioni generate contengono `seq` come sotto-sequenza.
* **Note**: Dato che con le correzioni date a voce sull'esercizio esso non richiede più di agire sul *Diabetes Dataset* e quindi di avere sequenze temporali, anziché agire su giorni ho agito direttamente sul numero di items nella sequenza e ho cambiato di conseguenza i nomi alle variabili. 

## Esercizio 2
* **Richiesta**: valutare quanto un elemento sia influente su una regola, relativamente a una misura di bontà che posso scegliere a piacere. Per questo esercizio si scelga la confidenza.

## Esercizio 3
* **Richiesta**: realizzare un oggetto `SequenceTree` che, dato un dataset, presenta due metodi:
  * `fit`: costruisce un albero di decisione che consuma sequence facendo test di evento ("esiste un evento di tipo label entro distanza temporale d") e di valore ("dato un testo di evento, il suo valore è maggiore o minore della soglia") per distinguere fra classe 0 e 1, e che calcola ciascun test come il test che massimizza l'information gain.
  * `predict`: dato un albero già allenato e un nuovo elemento, esegue i test dell'albero e assegna una classe all'elemento.

## Esercizio 4
* **Richiesta**: realizzare un classificatore di tipo boosting che usi come *weak classifier* un insieme di *sequence trunk*, ovvero *sequence tree* come definiti nell'esercizio precedente ma la cui struttura è limitata a un singolo test di evento e un singolo test di valore.

## Esercizio 5
* **Richiesta**: convertire il *boosting classifier* dell'esercizio precedente in un *conformal predictor*.