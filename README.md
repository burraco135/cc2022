# Calcolabilità e Complessità

Materiale per l'esame di calcolabilità e complessità 

## Teoria

### Teoremi
#### Teorema di Cook-Levine
#### Teorema di Savitch

### Definizioni
#### Automa a pila (PDA)
#### Automa deterministico (DFA)
#### Automa non deterministico (NFA)

### Dimostrazioni
#### Equivalenza fra NFA e DFA
#### {(M, w) | M è una mdT che accetta w} indecidibile
#### P chiusa rispetto a unione, concatenazione, complemento
#### P chiusa rispetto a intersezione e concatenazione
#### Linguaggio regolare se esiste espressione regolare
#### {M | M è una mdT e L(M)=&empty;} complemento Turing-riconoscibile
#### Linguaggi regolari chiusi rispetto a unione
#### SAT NP-completo
#### TRIANGLE in P, con TRIANGLE = {<G> | G contiene un triangolo}

## Esercizi
### {ww | w in {0, 1}\*} non è regolare
### PDA
### NFA (a|b)\*abb
### DFA (a(ab|bb)\*(aa|c))\*
### DFA {w in {0, 1}\* | w non contiene mai più di due 0 consecutivi}
### Linguaggio non Turing-riconoscibile
### Problemi NP
  
## Tracce
### Traccia 1
1. Dimostrare l'equivalenza fra NFA e DFA
2. Dimostrare che il linguaggio {(M, w) | M è una mdT che accetta w} è indecidibile
3. Dimostrare il teorema di Cook-Levine
4. Scrivere la definizioone di automa a pila (PDA), e definire il PDA che riconosce il linguaggio {a<sup>i</sup>b<sup>j</sup>c<sup>k</sup> | i, j, k &ge; 0 e (i = j oppure i = k)}
5. Scrivere il DFA che accetta stringhe nel linguaggio (a(ab|bb)\*(aa|c))\*
6. Dimostrare che P è chiusa rispetto a unione, concatenazione e complemento

### Traccia 2
1. Dimostrare che un linguaggio è regolare se e solo se esiste almeno una espressione regolare che lo descrive
2. Dato il linguaggio {M | M è una mdT e L(M)=&empty;}, dimostrare che il suo complemento è Turing-riconoscibile
3. Dimostrare il teorema di Savitch
4. Scrivere la definizione di DFA, di NFA, e definire il NFA che riconosce il linguaggio (a|b)\*abb
5. Fornire un esempio di problema in NP
6. Dimostrare che P è chiusa rispetto a intersezione e concatenazione

### Traccia 3
1. Dimostrare che la classe dei linguaggi regolari è chiusa rispetto all'operazione di unione (senza usare automi non deterministici)
2. Dato il linguaggio {ww | w in {0, 1}\*}, dimostrare che non è regolare
3. Fornire un esempio di linguaggio non Turing-riconoscibile e dimostrare perché
4. Dimostrare che SAT è NP-completo
5. Un triangolo in un grafo non orientato è una clique di dimensione 3; dimostrare che TRIANGLE è in P, con TRIANGLE = {<G> | G contiene un triangolo}
6. Scrivere il DFA che accetta il linguaggio {w in {0, 1}\* | w non contiene mai più di due 0 consecutivi}
