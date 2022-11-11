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
