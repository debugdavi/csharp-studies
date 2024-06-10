### Matriz Regular
- São arranjos com duas dimensões ou mais, sendo homogênea, ordenada e também alocada de uma vez, não podendo colocar ou tirar espaços depois de declarar e instanciá-la. 
- Para você declarar e instanciar uma matriz em c#, é da seguinte forma:
```
double[,] matriz = new double[4, 4]
```
	Ou seja, [,] serve para indicar que é um arranjo bidimensional, e na instanciação você só precisa colocar a quantidade de linhas e colunas dentro dos dois colchetes
#### Métodos das Matrizes
##### Length 
- Serve para dizer a quantidades de elementos que a matriz possui.
##### Rank
- Serve para retornar quantas dimensões existem na matriz.
##### GetLength
- Serve para dizer o tamanho de linhas e colunas(dimensões 0 e 1).
```
double [,] matriz = new double[5,8];
Console.WriteLine(matriz.GetLength(0));
```
- Na dimensão 0(linhas), ele vai retornar 5 e na dimensão 1(colunas), ele vai retornar 8;



### Matriz Irregular
- Para instanciar uma matriz irregular:
```
double[][] matriz = new double [10][];
```
- Nós só colocamos a quantidade de linhas que desejamos, depois disso a gente vai preenchendo as colunas conforme o necessário do usuário, podendo usar qualquer quantidade de colunas em cada linha. Por isso a matriz é irregular.
```
matriz[0][0] = 31.0;
matriz[0][1] = 32.0;
matriz[1][0] = 23.0;
matriz[1][1] = 52.0;
matriz[1][2] = 43.0;
```
![[Pasted image 20240516135516.png]]