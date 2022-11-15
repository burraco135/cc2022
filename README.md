# Calcolabilità e Complessità

Materiale per l'esame di calcolabilità e complessità

## Autori
- [Ester](https://github.com/burraco135)
- [Giacomo](https://github.com/GiacomoSignorile)

## Indice
- Teoremi
  - Cook-Levine
  - Savitch
- Macchine di Turing
  - Funzioni
    - (link) Sottrazione in modulo: `f(x,y) = |x-y|`
    - (link) Massimo: `f(x,y) = max(x,y)`
    - (link) Addizione a 2: `f(x,y) = x+y`
    - (link) Addizione a 3: `f(x,y,z) = x+y+z`
    - (link) Sottrazione tra positivi: `f(x,y) = x-y`
    - (link) Moltiplicazione: `f(x,y) = x*y`
    - (link) Incrementa: `f(x,y) = x+1`
  - Decisori
    - (link) `{ w in {0,1}* | #(1,w) = #(0,w) }`
    - (link) `{ w in {0,1,2}* | #(2,w) = #(1,w) = #(0,w) }`
    - (link) `{ a^n b^n c^(n+1) | n > 0 }`

## Teoremi
### Teorema di Cook-Levin
> Un problema decisionale appartiene a NP se una macchina di Turing non deterministica può calcolare la soluzione in tempo polinomiale.

Un problema decisionale è NP-completo se appartiene a NP e se ogni problema appartenente ad NP può essere ridotto ad esso in tempo polinomiale.
Un'istanza del problema di soddisfacibilità booleana è un'espressione booleana che combina variabili booleane usando degli operatori booleani. Un'espressione è soddisfacibile se c'è almeno un assegnamento di valori di verità alle variabili tale che l'espressione sia vera.

#### Dimostrazione
Si dimostra che il funzionamento di una macchina di Turing si può simulare tramite formule booleane in forma normale congiuntiva. Ogni problema che può essere risolto tramite una macchina di Turing può essere tramutato in una formula booleana e quindi il propblema di soddisfacibilità booleana è NP-completo.

1. SAT appartiene ad NP
2. Ogni linguaggio in NP è riducibile a SAT in tempo polinomiale

### Teorema di Savitch
> Se una macchina di Turing non deterministica è in grado di risolvere un problema in spazio f(n), una macchina di Turing deterministica può risolvere lo stesso problema nel quadrato dello spazio.

Un importante corollario del teorema è che PSPACE = NPSPACE; ciò deriva dal fatto che il quadrato di una funzione polinomiale è a sua volta una funzione polinomiale.

#### Dimostrazione
Il teorema di Savitch codifica attraverso un grafo orientato le configurazioni di una macchina di Turing. Ogni nodo del grafo rappresenta una configurazione. Tra due nodi u e v esiste un arco orientato se dalla configurazione u è possibile raggiungere la configurazione v.

Il problema di decidere un linguaggio si trasforma in un problema di raggiungibilità su grafi orientati. Nello specifico si tratta di capire se dalla configurazione iniziale è possibile raggiungere una qualunque configurazione di accettazione.

Viene presentato un algoritmo che in base ad una stringa w data come ingresso ad una macchina di Turing N, due configurazioni c_1 e c_2 ed un ingresso t, restituisce `true` se dalla configurazione c_1 è possibile raggiungere la configurazione c_2 in almeno t passi.
