Diferente do C, que o mod não funcionava com números ponto flutuante, no C# ele funciona, usando o casting tambem!
	`double n4 = 10.0 / 8;`
			ou
	`double n4 = double(10) / 8;`
		As duas retornam o valor de 1.25

Para você usar funções de bibliotecas, como eram chamadas no c, basta chamar algo do tipo Math.Pow(b, 2.0). onde Math eh a biblioteca chamada e Pow eh a função que você quer usar da biblioteca.
	`double delta = Math.Pow(b, 2.0) - 4.0 * a * c;`