### Inserir Elementos
```
list.Add();
```
- Essa função serve para adicionar elementos que sejam do tipo da lista, dentro dos parenteses você ia passar o seu elemento

```
list.Insert();
```
- Essa função serve para adicionar elementos que sejam do tipo da lista e também especificar o índice que você quer que fique o seu elemento! ex: `list.insert(2, "Joao");`
### Tamanho da Lista
```
list.count();
```
- Essa função passa o tamanho da lista.
### Encontrando elementos
```
list.Find(expressão lambda ou função)
```
- A gente passa um predicado como parâmetro(expressao lambda), e se ele achar um valor que atenda a essa expressão, o método Find retorna ele. No método Find, ele pega a primeira ocorrencia encontrada.
```
list.FindLast(expressão lambda ou função)
```
- A gente passa um predicado como parâmetro(expressao lambda), e se ele achar um valor que atenda a essa expressão, o método Find retorna ele. No método Find, ele pega a ultima ocorrencia encontrada.
`list.FindIndex();`
- Aqui é na mesma linha de raciocinio do list.Find(), só que ao invés de retornar o elemento, ele vai retornar o index(posição dele). Ele vai pegar a primeira ocorrencia que atenda o predicado e retornar o index.
`list.FindLastIndex();`
- Aqui é na mesma linha de raciocinio do list.FindLast(), só que ao invés de retornar o elemento, ele vai retornar o index(posição dele). Ele vai pegar a última ocorrencia que atenda o predicado e retornar o index.
### Filtrando lista e criando uma nova de acordo com o predicado
`list.FindAll()`
- Para usar esse método, é necessário criar uma nova lista e depois atribuir a lista antiga com esse método, passando o predicado que atenda os seus requisitos. Assim ele cria uma lista de elementos que atendam somente ao escopo que você definiu. Ex: `list<string> list2 = list.FindAll(x => x.Length == 5);`

### Removendo elementos da lista
`list.Remove();`
- Ele remove o elemento que você passou no parâmetro.
`list.RemoveAll(predicado);`
- Ele remove todos os elementos que atendem ao predicado que você passou.
`list.RemoveAt(index);`
- Ele remove o elemento através do index que você passar.
`list.RemoveRange(index, contagem);`
- Ele remove o elemento a partir do index que você passou e no outro parâmetro a quantidade de elementos que você quer remover a partir do index em diante.
