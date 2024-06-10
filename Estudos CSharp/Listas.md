### Definição
- São arranjos unidimensionais, vazios, homogêneos e alocados sob demanda, ou seja. Ele não vai ser pronto como vetor na instanciação dele, como exemplo: 
```
int[] vetor = new int[20];
```
- Aqui em cima, o vetor só pode ter 20 espaços de memória para inteiros, sem poder adicionar ou remover esses espaços. Na lista você adiciona conforme você precisa, sem precisar dizer quantos espaços você vai utilizar.
### Para poder usar:
- Para usar é necessário que antes do código em si você coloque:
```
using System.Collections.Generic;
```
- E no código você põe:
```
List<tipo> listinha = new List<tipo>;
```
- Exemplo:
```
List<string> listinha = new List<string>;
```

### Desvantagem
- Pense que você tem uma lista de 100 espaços, para acessar a posição 50, você tem que percorrer a lista até chegar no espaço 50, ou seja o acesso é sequencial.