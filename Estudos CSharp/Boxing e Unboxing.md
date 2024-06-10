### 1.1 - Boxing
- É o processo de conversão de um objeto tipo valor para um objeto tipo referência.(Tudo em c# deriva da classe Object).
```
int x = 20;

Object obj = x; 
```
- O int x vai guardar o valor iniciado na stack, enquanto o obj vai guardar um valor de memoria da heap onde está o valor iniciado.

### 1.2 - Unboxing
- É o processo de conversão de um objeto tipo referência para um objeto tipo valor.
```
int x = 20;

Object obj = x; 

int y = (int) obj;
```
- Para a transformação de um object para struct, é necessário utilizar o casting que seja compatível com o valor guardado no "obj"