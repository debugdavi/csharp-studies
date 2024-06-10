### Definição
- Em síntese, os dois vão ser responsáveis por criarem referências diretas a uma variável do tipo valor. A única diferença entre a ref e a out, é que a ref precisa ser inicializada, enquanto a out não precisa.
### Exemplos - REF
```
int a = 10;
Calculator.Triple(ref a);




public static void Triple(int ref x){
	x = x * 3;
}
```
- Você nota que na primeira parte, na chamada do método, é necessário colocar o ref a, dizendo que está passando uma referência de variável como parâmetro para o método(como se estivesse passando a original). E também no método, note que ele pede uma referência de um inteiro para poder realizar a operação, que é triplicar o número. Dessa forma, o método vai manipular o número(daquela referencia) em si, não mexer só naquele escopo.

### Exemplos - OUT
- Aqui a gente pode usar o out para guardar resultados da saída de alguma operação, como já diz na própria tradução do OUT, que é saída. 
```
int a = 10; 
int triple; 
Calculator.Triple(a, out triple); 
Console.WriteLine(triple);

public static void Triple(int origin, out int result) { 
	result = origin * 3; 
}
```