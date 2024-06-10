- São membros que fazem sentido sem depender de objetos. Não precisam de objetos para serem chamados, porém são chamados a partir do nome da classe. 

- Metodo de classe <=> Metodo Estaticos

- Membros de instancia sao aqueles presentes nos diagramas UML para criação de classes

- ==Ex:== Classes Utilitarias(ao chamar o `Math.Sqrt()`, voce não precisou do objeto Math, você chamou a classe e pediu o método) e declaracao de Constantes

- Uma classe que so possui membros estaticos, pode ser uma classe estatica, implicando nela não poder ser instanciada

- ==Não é possível chamar uma função não estática dentro de uma função estática na mesma classe== (obs: criando variaveis fora de membros na classe tambem eh necessario declarar usando o static, como `static double Pi = 3.14;`)

- Se você fizer um objeto Calculadora, com metodos de calcular circuferencia e volume, e instanciar dois objetos, note que os resultados vão ser os mesmos(se dados a mesma entrada), por isso é melhor uma abordagem usando a classe estática.

- Note, que para criar uma classe estática, de forma que ela funcione igual o Math, todos os membros, sejam metodos ou atributos, tem que estar com o prefixo `static`. Dessa forma, a classe não vai precisar ser instanciada para chamar os seus métodos ou atributos.