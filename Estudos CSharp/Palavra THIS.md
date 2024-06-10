Eh a referencia para o proprio objeto

##### Usos comuns
- Diferenciar atributos de variaveis locais(mais comumente usado no Java por causa do camelCase)
- Referenciar outro construtor em um construtor
- Passar o próprio objeto como argumento na chamada de um metodo ou construtor
- Heap x Stack

### Referenciar construtor em outro construtor

`public Produto() {`
	`Quant = 0 ;`
`}`


`public Produto(string nome, double preco) : this(){`
    `Nome = nome;`
    `Preco = preco;`
`}`

<p> 
Observe que o this( ) está colocado no segundo Construtor de Produtos, o this() utilizado desssa forma vai servir para executar o construtor PADRÃO da classe, aproveitando assim a inicialização de um produto com quantidade = 0.

![[Pasted image 20240416103245.png]]

Veja neste exemplo.  Note que no terceiro construtor da classe Produto, temos uma referencia a outro construtor, qual seria? Seria o construtor Produto(string nome, double preco)! Note tambem que no c3, nós recebemos três parametros, mas ele usa a assinatura do segundo construtor para isso, e no c3 só faz a operacao de Quant =  quantidade. Aqui fica claro o reaproveitamento de código!
<p/>
### Passar proprio objeto como argumento na chamada de um metodo ou construtor

Confesso que essa parte eu não entendi, mas mais pra frente eu entenda!

Class ChessMatch{
	PlaceNewPiece('e', 1, new King(board, Color.White, this));
}