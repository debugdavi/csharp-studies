### Toda classe em C# é uma subclasse da classe Object, e ele possui os seguintes metodos: 
- GetType
- Equals
- GetHashCode
- ToString


----------------
# Antes colocando um objeto dentro de um writeline, o compilador mostrava o namespace.objeto:
`Console.WriteLine("Dados do produto " + p)`
Ele retornava ProdutosTest.Produto (ou seja, namespace.objeto)

-------
## Para resolver isso, a gente reescreve o metodo ToString da classe Produtos, da seguinte forma:

`override string ToString(){
	`return Nome + ", $ " + Preco;`
`}`

Assim, toda vez que colocarmos o WriteLine, ele retorna de acordo com os dados pedidos e formatados pelo usuario, colocando apenas o nome do objeto, sem precisar formatar o WriteLine

