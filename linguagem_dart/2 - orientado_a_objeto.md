# Dart e Orientação à objeto.

Dart é uma linguagem que suporta todos os conceitos da orientação objeto, como:

 - Classes
 - Objetos
 - Herança
 - Mixin
 - Abstração de classes

#### O modelo de orientação objeto, sugere criar uma classe que represente todas as informações e ações necessárias para se comparar a ela na vida real.

Vamos criar uma classe que represente um cliente de banco, com os atributos e comportamentos necessários para o nosso banco:

 - Nome
 - Telefone
 - Email
 - CPF
 - Saldo
 - Cartão de Crédito

```dart
class clienteBanco {
    final String nome;
    final String telefone;
    final String email;
    final String cpf;
    final double saldo;
    final double cartaoDeCredito;
}

```