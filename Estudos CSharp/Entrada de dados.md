## STRING
Para fazer a leitura de dados, se utiliza o Console.ReadLine(), ele retorna os dados em STRING. Ele funciona de uma forma semelhante do input do python:
	`string frase = Console.ReadLine();`
	
Por exemplo, quando você quer colocar tres objetos dentro de três variáveis(p1, p2, p3) usando apenas uma linha, você tem que usar o metodo Split(), não é parecido igual o C, que você dava espaço e ele achava que cada um era quebra de linha pra responder o scanf. Neste caso você faz da seguinte maneira:

	`string S = Console.ReadLine();`
		\\"batata tomate abacaxi"
	`string[] vet = s.Split(' ');`
		\\Tambem eh possivel fazer da seguinte forma
	`string[] vet = Console.ReadLine().Split('')`

Nesse ultimo comando, acabei de criar um vetor de string, que vai pegart a variavel s e dividir ela a cada caractere de ' ', ficando separado e guardado na memoria o 0 = batata, 1 = tomate, 2 = abacaxi.
	Para terminar o que foi solicitado de guardar cada um desses em uma variavel, a gente só faz o seguinte:
	`string p1 = vet[0];`
	`string p2 = vet[1];`
	`string p3 = vet[2];`

## Números, char, etc
Para você ler numeros, voce faz da seguinte forma: 
	`int n1 = int.Parse(Console.ReadLine());`

Para ler um char:
	`chat g = char.Parse(Console.ReadLine());`

Para ler um ponto flutuante:
	`double flu = double.Parse(Console.ReadLine());`
	Note que aqui você deve responder usando virgula no seu ponto flutuante e não ponto, como eh de costume, você deve usar aquele mesmo negocio do CultureInfo.InvariantCulture, fazendo assim:
	`Using System.Globalization;`
	`double d = double.Parse(Console.ReadLine(), CultureInfo.InvariantCulture);`
