- Recurso que uma classe possui de oferecer mais de uma operacao com o mesmo nome, porem com diferentes listas de parametros.

- Nisso, as ==classes== podem sim ter uma sobrecarga, ou seja, classes podem receber mais de um construtor. Por exemplo, uma classe Produtos, com construtores (nome, preco, quantidade) e (nome, preco). Desta forma o segundo construtor vai inicializar o Quant no 0.

- Note que depois de criar os construtores, voce nao pode mais usar o construtor padrao(Produtos p1 = new Produtos( )). Mas caso queira, voce pode realizar outra sobrecarga de construtor, com parametros e chaves vazios. Ex: public Produtos(){}.