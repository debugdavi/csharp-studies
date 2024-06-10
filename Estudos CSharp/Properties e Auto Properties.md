## Properties
Properties vão ser acessadores e funcionarão como métodos públicos, facilitando e tornando mais flexível o uso do encapsulamento, só que de uma forma mais amigável.

![[Pasted image 20240416112319.png]]

Isso é um exemplo de uma property. Cada atributo deve receber um dependendo do uso dele. Note que o get é bem simples, já o set ele tem um ponto que é necessário atenção. Lembra que quando usamos o set numa encapsulação comum era necessário um parâmetro? Pois bem, o value vai agir nesse sentido, só que ao invés de você fazer Produto._nome = value, você vai fazer Produto.Nome = value; (No programa principal)

## Auto Properties
As auto properties vão valer a pena em casos em que não há uma lógica específica para atribuição de valores, como tem na imagem acima uma lógica para isso. Através das auto properties você não vai precisar declarar lá em cima uma variável e depois precisar fazer uma property pra ela, você pode fazer os dois de uma vez lá no início nos atributos, da seguinte forma:
![[Pasted image 20240416113729.png]]\
Assim você dispensa as properties implementadas posteriormente, deixando o código mais limpo e organizado. Um adendo é que você vai precisar alterar seu código, utilizando o nome "Preco" e "Quant"(como está definido nas properties) nas operações da classe. O private vc coloca quando você não vai alterar!

- Um adendo, quando você coloca um private set numa property, voce so pode alterar o valor da variavel atraves de metodos dentro da propria classe!