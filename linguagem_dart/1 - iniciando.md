# Introdução a Dart.

# Primeiro código rodando.
### Todo aplicativo deve conter a função main, onde será iniciada a execução do programa.
#### Esse função não retorna nenhum tipo de valor (void)

No exemplo abaixo vamos mostrar no console a frase "Olá Mundo".

```dart
void main() {
  print('Olá Mundo!');
}
```

# Váriaveis

### Mesmo sendo *type-safe* 
(tipo seguro, quando a linguagem sabe qual o tipo de valor que irá receber)

#### No dart podemos criar váriaveis com o tipo explicito ou implicito

```dart
// implicito
final appName = 'Museu Histórico de Campos dos Goytacazes';

// explicito
final String appName = 'Museu Histórico de Campos dos Goytacazes';
```

#### Devemos tomar cuidado ao tratar os tipos, pois há funções que trabalham apenas com um tipo especifico de dado.

A função abaixo printInts só consegue receber uma lista de inteiros, como no exemplo abaixo

```dart
void printInts(List<int> a) => print(a);

void main() {
  final list = <int>[];
  list.add(1);
  list.add(2);
  printInts(list);
}
```

Ao tentar passar algum valor que não seja inteiro vc receberá um erro de compilação.

Esse é um dos beneficios do soundness

 - Revelar bugs em tempo de execução
 - Código mais fácil de ler
 - Maior fácilidade de manter o código, ao se alterar pequenos pedaços de código o debug te avisa em tempo real se o tipo do valor da váriavel estiver errado.
 - Código mais eficiente em AOT (Tempo de pré compilação, evitando vc ter um problema de tipo em faze de execução).