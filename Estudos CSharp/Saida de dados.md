- `Console.WriteLine("Boas noites")`, esse exibe o que tá escrito com uma quebra de linhas
- `Console.Write("Boas noites")`, esse imprime o que está escrito mas sem quebra de linhas

## Para escrever variaveis na tela

- Console.WriteLine('nome da variavel'), basicamente isso, mas no caso da variavel do tipo ponto flutuante(float double ou decimal), pode acontecer de querer uma formatação, dessa forma, a gente pode seguir da seguinte maneira:
		`double saldo = 10.32144;`
		`Console.WriteLine(saldo.ToString("F2"))`
		Ou seja, você precisa usar o ToString, e entre aspas, voce coloca um F e escolhe o numero de casas decimais que voce quer deixar

- Para você fazer a saida usando o ponto normal, você precisa colocar:
	- `Using namespace System.Globalization;`
		Apos isso, voce vai la onde voce quer colocar o ponto e no segundo parametro do ToString, coloca CultureInfo.InvariantCulture. ficando assim:
	- `Console.WriteLine(saldo.ToString("F2", CultureInfo.InvariantCulture))`

## Placeholders, concatenação e interpolação

- Placeholders:
		`Console.WriteLine("{0} fodido tem exatos R${1} na conta, aos {2} de idade, falido!", _nome, _saldo, _idade);`
		Para formatar a quantidade de casas do saldo, faça {1:F2}, para determinar a quantidade de casas na variavel na posição 1

- Interpolação
		`Console.WriteLine($"{_nome} fodido tem exatos R${_saldo:F2} na conta, aos {_idade} de idade, falido!");`
		Note que da mesma forma que você formatou no placeholders, usando numeros, vc pode fazer na interpolação, usando o nome da variavel!

- Concatenação
		`Console.WriteLine("A paciente " + z + " tem " + y + " anos e seu sexo é: " + w);`

