# Local-Algorithm-Alignment
## Autores: Luís Filipe Loureiro e Murilo Lima

O algoritmo foi construído com base na aleatoriedade. Para tanto, foi baseado no gerador randômico do cpp.

Após o recebimento das entradas: tamanhos e as prórpias strings de DNA (`seqA` e `seqB`) é criado um número randômico `int k`. Ele representa o tamanho da substring
que será recortado da  `seqB`. Ou seja, é respeitado a ordem da string, sendo apenas realizado um recorte do início até `k`. Importante salientar que foi definido que o tamanho máximo de `k` é o tamanho de `seqA`.

Em seguida, é gerado um segundo valor aleatório, `int p`. Esse é o número de substrings que serão criados a partir da `seqA`, com tamanho `k`. Para tanto,
os recortes foram iniciados no início de `seqA` e vão de um e um.

Por fim, é comparado as substrings de `seqA` com `seqB`, considerando os seguintes valores para cada letra:

 | Comparação  |Resultado |
| ------------- | ------------- |
| iguais  | 2 |
| diferentes  | -1  |


Indentificando, assim, a substring de A que tinha seu valor total maximizado.
