## Definição
Tipo enumerado especial que define três valores possíveis para localidade da data.
- Local(fuso horário do sistema)
- UTC(fuso horário GMT - Greenwich Mean Time)
- Unspecified

### Boas práticas
- Armazenar data em formato UFC(texto - BD/ JSON / XML)

- Para mostrar para o usuário você deve instanciar e mostrar no formato local. Para converter um DateTime para Local ou UTC, é necessário usar
```
myDate.ToLocalTime(); -> Data da maquina

myDate.ToUniversalTime(); -> Data universal
```

### DataTime.Kind()
- Função que retorna se o objeto DateTime está no horário local ou no horário universal(UTC)

## Padrão ISO 8601
- É um padrão universal de representar horários e datas. No seguinte formato =="yyyy-MM-ddTHH:mm:ssZ"==. 
- Quando você instancia um objeto DateTime nesse formato, note o seguinte.
- ![[Pasted image 20240523143110.png]]
- Quando você pedir para a variável ser exibida, ele vai mostrar o horário no fuso local da sua máquina. O horário armazenado vai ser em UTC, mas quando ela for instanciada e mostrada, vai ser em forma local.

Para você imprimir uma data nesse formato, você deve passar para o formato universal e depois para o ToString com a máscara de formatação mostrada lá em cima.
```
Console.WriteLine(d2.ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ssZ"));
```