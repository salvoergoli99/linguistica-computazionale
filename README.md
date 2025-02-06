# linguistica-computazionale
Progetto Linguistica Computazionale - Anno accademico 2022/2023
# Progetto 1
Il codice sviluppato deve prendere in input i due corpora, effettuare le operazioni di
annotazione linguistica richieste (sentence splitting, tokenizzazione, PoS tagging,
lemmatizzazione), e produrre un confronto dei corpora rispetto a:
1) Numero di frasi e token;
2) Lunghezza media delle frasi in token e lunghezza media dei token, a eccezione della
punteggiatura, in caratteri;
3) Numero di Hapax tra i primi 500, 1000, 3000 token, e nell’intero corpus;
4) Dimensione del vocabolario e ricchezza lessicale (Type-Token Ratio, TTR), calcolata
per porzioni incrementali di 200 token (i.e., i primi 200, i primi 400, i primi 600, …);
5) Numero di lemmi distinti (i.e., la dimensione del vocabolario dei lemmi).
# Progetto 2
Il codice sviluppato deve prendere in input un corpus, effettuare le operazioni di
annotazione richieste (sentence splitting, tokenizzazione, PoS tagging), ed estrarre le
seguenti informazioni:
1) La sequenza ordinata per frequenza decrescente, con relativa frequenza, di:
a. 10 PoS, bigrammi di PoS, e trigrammi di PoS più frequenti
NB: risolvere il problema con una singola funzione che prenda in input il
valore di n
b. 20 Sostantivi, Avverbi, e Aggettivi più frequenti
NB: risolvere il problema con una funzione che filtri la lista di (token, PoS)
prendendo in input la lista e la/le PoS su cui filtrarla
2) Estratti i bigrammi composti da Aggettivo e Sostantivo mostare:
a. I 20 più frequenti, con relativa frequenza
b. I 20 con probabilità condizionata massima, e relativo valore di probabilità
c. I 20 con forza associativa (Pointwise Mutual Information, PMI) massima, e
relativa PMI
3) Considerate le frasi con una lunghezza compresa tra 10 e 20 token, in cui almeno la
metà (considerare la parte intera della divisione per due come valore) dei token
occorre almeno 2 volte nel corpus (i.e., non è un hapax), si identifichino:
a. La frase con la media della distribuzione di frequenza dei token più alta
b. La frase con la media della distribuzione di frequenza dei token più bassa
c. La frase con probabilità più alta secondo un modello di Markov di ordine 2
costruito a partire dal corpus di input
NB: la media della distribuzione di frequenza dei token è data dalla somma
delle frequenze (nel corpus) dei token della frase diviso il numero di token
della frase
4) Estratte le Entità Nominate del testo, identificare per ciascuna classe di NE i 15
elementi più frequenti, ordinati per frequenza decrescente e con relativa frequenza.
