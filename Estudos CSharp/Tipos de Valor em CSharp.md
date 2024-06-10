Tipos mais utilizados:
	1. int
	2. long (numeros inteiros grandes)
	3. float(é necessário inicializar o float da seguinte forma  ==float num = 3.43f==, com o f no final indicando que é float )
	4. double (mais preciso que o float)
	5. decimal (mais preciso que o double)
	6. char (funciona de forma similar no c) => **PARA PASSAR UM CARACTERE UNICODE POR NUMERO, VOCÊ USA ANTES DO NÚMERO '==\\u0000=='**
	7. bool (existe no c#)
	8. string (SIM AMEM, (string frase = "Deus nunca abandona."))
	9. object, variavel que recebe qualquer tipo de dado

Tipos somente positivos
	1. byte
	2. ushort
	3. uint
	4. ulong


Overflow: Quando um valor ultrapassa o tamanho aceito pela variavel. Uma curiosidade é que quando acontece um overflow, ele volta para o limite oposto(negativof)

Para descobrir valores minimos e maximos dos tipos
	Basta colocar o tipo e chamar a função .MinValue ou .MaxValue, ex:
		1. int.MinValue
		2. sbyte.MaxValue
		3. etc