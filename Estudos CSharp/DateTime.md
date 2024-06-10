- Representa um INSTANTE • É um tipo valor (struct) 
https://msdn.microsoft.com/en-us/library/system.datetime(v=vs.110).aspx 

- Um objeto DateTime internamente armazena: O número de "ticks" (100 nanosegundos) desde a meia noite do dia 1 de janeiro do ano 1 da era comum
- Para o DateTime retornar a data atual, ele guarda esses ticks e depois faz um calculo para gerar ela.

### Funcoes importantes
- DateTime.Now 
- DateTime.UtcNow 
- DateTime.Today [time: 00:00:00] 
- DateTime.Parse(string) 
- DateTime.ParseExact(string, string)

### Propriedades do DateTime
- Ele também possui muitas propriedades que podem ser chamadas na variável. Podendo mostrar dia da semana, dia do ano, o mes, o dia, tudo bem separadinho só chamando as propriedades da forma correta!
- ![[Pasted image 20240521144419.png]]
```
DataTime data = new DataTime(2001, 8, 15, 13, 45, 58, 423);
Console.WriteLine("Dia: {0}", data.Day);
```
### Operações com DateTime
- Há muitas operações, para adicionar minutos, horas, dias e entre outros. Também é possível comparar e afins. aqui está um print e o link que mostra a maioria.
- ![[Pasted image 20240521145902.png]]
- [DateTime Struct (System) | Microsoft Learn](https://learn.microsoft.com/en-us/dotnet/api/system.datetime?view=net-8.0&redirectedfrom=MSDN)
