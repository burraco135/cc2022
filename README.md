# Calcolabilità e Complessità

Materiale per l'esame di calcolabilità e complessità

## Indice
- [Teoremi](#teoremi)
  - Cook-Levine
  - Savitch
- [Macchine di Turing](#macchine-di-turing)
  - Funzioni
    - Sottrazione in modulo: `f(x,y) = |x-y|`
    - Massimo: `f(x,y) = max(x,y)`
    - Addizione a 2: `f(x,y) = x+y`
    - Addizione a 3: `f(x,y,z) = x+y+z`
    - Sottrazione tra positivi: `f(x,y) = x-y`
    - Moltiplicazione: `f(x,y) = x*y`
    - Incrementa: `f(x,y) = x+1`
  - Decisori
    - `{ w in {0,1}* | #(1,w) = #(0,w) }`
    - `{ w in {0,1,2}* | #(2,w) = #(1,w) = #(0,w) }`
    - `{ a^n b^n c^(n+1) | n > 0 }`

## Teoremi
### Teorema di Cook-Levine
### Teorema di Savitch

## Macchine di Turing
### Funzioni
#### Sottrazione in modulo: `f(x,y) = |x-y|`
![sottrazione_unaria_modulo](https://user-images.githubusercontent.com/64893048/201385766-715078f7-0728-43d0-b3d7-4338701f52de.png)

![sottrazione_binaria_modulo](https://user-images.githubusercontent.com/64893048/201387757-e478c577-9b6c-4efd-b71f-a87a6000033f.png)

#### Massimo: `f(x,y) = max(x,y)`
![massimo_unario](https://user-images.githubusercontent.com/64893048/201388522-47c1346d-1925-461c-97bc-5deea6c92ce9.png)

![massimo_binario](https://user-images.githubusercontent.com/64893048/201389320-4f02a8f6-147f-43cf-b3ea-bb810f73682e.png)
