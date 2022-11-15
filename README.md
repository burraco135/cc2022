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
    - (link) Massimo: `f(x,y) = max(x,y)` (link)
    - (link) Addizione a 2: `f(x,y) = x+y` (link)
    - (link) Addizione a 3: `f(x,y,z) = x+y+z` (link)
    - (link) Sottrazione tra positivi: `f(x,y) = x-y` (link)
    - (link) Moltiplicazione: `f(x,y) = x*y` (link)
    - (link) Incrementa: `f(x,y) = x+1` (link)
  - Decisori
    - (link) `{ w in {0,1}* | #(1,w) = #(0,w) }` (link)
    - (link) `{ w in {0,1,2}* | #(2,w) = #(1,w) = #(0,w) }` (link)
    - (link) `{ a^n b^n c^(n+1) | n > 0 }` (link)

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

## Macchine di Turing
### Funzioni
#### Sottrazione in modulo: `f(x,y) = |x-y|`
![sottrazione_unaria_modulo](https://user-images.githubusercontent.com/64893048/201385766-715078f7-0728-43d0-b3d7-4338701f52de.png)

![sottrazione_binaria_modulo](https://user-images.githubusercontent.com/64893048/201387757-e478c577-9b6c-4efd-b71f-a87a6000033f.png)

#### Massimo: `f(x,y) = max(x,y)`
![massimo_unario](https://user-images.githubusercontent.com/64893048/201388522-47c1346d-1925-461c-97bc-5deea6c92ce9.png)

![massimo_binario](https://user-images.githubusercontent.com/64893048/201389320-4f02a8f6-147f-43cf-b3ea-bb810f73682e.png)

#### Addizione a 2: `f(x,y) = x+y`
![somma_unaria](https://user-images.githubusercontent.com/64893048/201390173-92db6af6-774d-4e5b-93dc-d95488d74203.png)
![somma_binaria](https://user-images.githubusercontent.com/64893048/201392850-ac21e0e2-f39e-433b-89a0-d6fad6a2c7b9.png)

#### Addizione a 3: `f(x,y,z) = x+y+z`

#### Sottrazione tra positivi: `f(x,y) = x-y`
![sottrazione_unaria](https://user-images.githubusercontent.com/64893048/201394056-ad25126f-2a36-497e-b03c-a523d5502034.png)
![sottrazione_binaria](https://user-images.githubusercontent.com/64893048/201394517-efcd2ede-7a2f-4a4b-88c8-f8fd6e7ca341.png)

#### Moltiplicazione: `f(x,y) = x*y`
![moltiplicazione_unaria](https://user-images.githubusercontent.com/64893048/201396046-683436f3-f34d-4372-8c50-24eda73686f7.png)
![moltiplicazione_binaria](https://user-images.githubusercontent.com/64893048/201398396-a5056b5e-a98a-4739-95c8-ac232e4526d4.png)

#### Incrementa: `f(x,y) = x+1`

![incrementa_binario](https://user-images.githubusercontent.com/64893048/201399058-d843ec2a-5e2e-476c-a403-9cf83ded2c3d.png)
