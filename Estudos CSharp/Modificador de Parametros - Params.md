### Problemática
- Suponha que você está criando uma calculadora em c# usando POO, você nisso vai se deparar que para cada tipo de soma(2, 3, 4 ou mais números), você vai ter que criar construtores para passar os números para o objeto para que aconteça a soma. Só que à medida que você põe mais números, você precisa também criar mais construtores, e isso é um trabalho que não vale a pena porque não é otimizado e acaba sendo bastante pesado.
![[Pasted image 20240502143706.png]]
### Solução
- É possível solucionar esse problema passando um vetor de números como parâmetro na classe!
![[Pasted image 20240502144148.png]]
- Note que também é bem chatinho passar parâmetros no código principal, como mostra na primeira imagemzinha, por causa da instância do vetor e das chaves. Para resolver isso, basta colocar o modificador de parâmetros ==params== no metodo de soma
![[Pasted image 20240502144412.png]] ![[Pasted image 20240502144420.png]]
- Assim, você só passa os números como se fossem contatos os numeros que voce precisa no construtor!