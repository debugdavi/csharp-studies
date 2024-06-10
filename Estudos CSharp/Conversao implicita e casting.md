- É possível fazer uma conversão implicita de um float para um double. Veja o exemplo
		`float a = 5.4f;`
		`double b = a;`
		==Isso é possível, mas agora colocar um valor double dentro de um valor float não, isso porque o tipo float armazena valores até 4 bytes, e o valor double armazena valores de 8 bytes, é como se estivessemos tentando colocar 8 bytes dentro de 4 bytes==. Devido a isso você pode acabar perdendo conteúdo da variável double, mas você, se tiver certeza que não está perdendo nada, você pode fazer da seguinte maneira:
			`double a;`
			`float b;`
			`a = 5.23;`
			`b = (float)a`
		O nome desse processo de conversão é casting

	