## Tipos referencia
- Classes são tipos referência. Exemplo:
`Product p1;`
- p1(stack) na verdade vai estar guardando o endereço da memória(heap) onde estão guardados os atributos dela. Tanto que se você tivesse uma variavel do tipo Product e atribuisse a ela o p1( p2 = p1), o p2 iria passar a apontar o que o p1 aponta, no caso para o endereço de memoria que estão os atribudos
### Valor null
- Tipos referencia aceitam a atribuição do valor "null", indicando que ela não aponta para lugar nenhum

## Tipos Valor
- Structs são tipos valor. Exemplo:
`double x;`
- x vai estar guardando o valor ponto flutuante qualquer(na memoria stack), sem passar referencia de nada. Se eu tivesse um x atribuido a y, y iria receber uma copia do valor de x.

### Structs
- Assim como você fazia em C, você pode fazer novos tipos em C#, atraves das structs, que são bem parecidas com as classes!
- Depois de criado sua struct em C#, você deve inicializar ela no arquivo principal! Você pode fazer isso de duas formas.
```
Point p;
p.y = 10.0;
p.x = 10.0;

Point p = new Point();
(aqui os valores serão inicializados com 0)
```

## Valores Padrão

- Quando alocamos(new) qualquer tipo estruturado(classe, struct, array) são atribuídos valores padrão aos seus elementos:

| numeros | 0                  |
| ------- | ------------------ |
| bool    | false              |
| char    | caractere codigo 0 |
| objeto  | null               |

