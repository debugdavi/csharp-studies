- É um recurso do c# para que dados de tipo valor(structs) possam receber o valor null. Por exemplo, em casos de preenchimento de dados opcionais.(Ou seja, comumente, variaveis tipo valor não recebem podem receber como valor inicial o null, então, para poderem receber, há esse recurso do c#)

- Para então fazer uma atribuição de um valor nulo a uma variável, fazemos das seguintes formas:
![[Pasted image 20240501142035.png]]
- Usar a primeira notação gasta mais tempo, um simples interrogação depois do tipo da variavel é bem mais simples.

### Métodos Padrão do Nullable
#### GetValueOrDefault
![[Pasted image 20240501142831.png]]
- Se a variável Y possuir um valor atribuído a ela que não seja nulo, o método vai retorná-lo. Porém, caso não haja, o método vai retornar o valor padrão de inicialização do tipo da variável.
#### HasValue
![[Pasted image 20240501143358.png]]
- O método verifica se a variável possui um valor não nulo, retornando um valor booleano. Caso tenha um valor nulo, retorna TRUE, caso não, retorna FALSE.
#### Value
![[Pasted image 20240501143552.png]]
- O método vai tentar imprimir o valor da variável, independente se tem um ou não. Caso não tenha, o compilador vai lançar uma exceção, mostrando que não há um valor na variável.

### Operador de Coalescência Nula

![[Pasted image 20240501144156.png]]
- O operador vai servir para quando quisermos atribuir um valor nullable a uma variável comum, mas quando no caso da variavel nullable ser nula, ela vai atribuir o valor depois dos "??". Achei uma sacada de genio.

