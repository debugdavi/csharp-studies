- Operacao especial da classe no momento da instanciacao do objeto. Ex: "Produto p1 = new Produto()", so que vao ter parametros exigidos pelo construtor, e voce vai colocar eles no parenteses

- Serve para iniciar valores dos atributos, permitir/obrigar que o objeto receba dados/dependencia no momento da instanciacao

- Se um construtor nao for especificado voce pode usar o construtor padrao, "Produto p1 = new Produto()"

- ==Eh possivel especificar mais de um construtor na mesma classe(sobrecarga)==

### Discussao de Melhoria
- Quando instanciamos um objeto sem construtores, ele vai ter os seus atributos nulos ou zerados. Isso faz sentido? De forma alguma né, diante disso você ve a importancia dos contrutores. 

- Para criar o construtor, voce vai fazer da seguinte forma:
  1. Colocar apos os atributos
  2. Digitar "public `NomeClasse` (atributos da classe no minusculo)". Exemplo `public Produto(string nome, double preco, int quantidade)`
  3. Na chave voce vai atribuir esses valores que a classe recebe ao objeto. `Nome = nome, Preco = preco, Quantidade = quantidade`