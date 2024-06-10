`Produto p = new Produto{
	`Nome = "TV",
	`Preco = 900.00,
	`Quantidade = 0
`};`

ou

`Produto p2 = new Produto(){
	`Nome = "TV",
	`Preco = 900.00,
	`Quantidade = 0
`};`

##### Observação
É possível utilizar essa abordagem mesmo quando a classe não tiver construtores definidos. E tambem deve ter a sobrecarga do construtor vazio ou nao pode ter outros construtores.