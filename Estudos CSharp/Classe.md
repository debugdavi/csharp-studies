- É um tipo estruturado aque pode conter membros, sendo eles, seus atributos(que são dados mais simples) e seus métodos(que são as funções/operações que executam)

# A classe tem recursos:
- Construtores
- Sobrecarga
- Encapsulamento
- Herança
- Polimorfismo

## Exemplos 
- Entidades: Produtos, Clientes, Triangulo
- Servicos: ProdutoService, ClienteService
- Controladores: ProdutoController, ClienteController
- Utilitarios: Calculadora, Compactador
- Outros(views, repositorios, gerenciadores, etc)

### Para criar classes é recomendado a boa prática de usar o inicio com letra maiuscula e o nome dos atributos da mesma forma. 

- Atributo public quer dizer que os atributos de uma classe podem ser acessados por outros arquivos.

## Depois de declarar as variaveis(classes novas), eh necessario instanciar elas no código!!! Da seguinte forma:
`Triangulo a = new Triangulo();`

## Stack e Heap
- Variaveis estaticas sao criadas dentro da memoria Stack
- Classes são instanciadas dentro da memoria HEAP(area de alocação dinamica), o nome da variavel da classe(por exemplo, Triangulo x), o x vai ficar na stack com o endereço de memoria que leva ate a Heap

## Para acessar os atributos, basta colocar o nome da variavel da sua classe:
`Triangulo x = new Triangulo();`
`x.A = double.Parse(Console.ReadLine(), CultureInfo.InvariantCulture);

##  CLASSE X OBJETOS
- Classes são definicoes de tipos
- Objetos são instancias dessa classe