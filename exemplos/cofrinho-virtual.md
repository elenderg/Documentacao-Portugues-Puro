# Cofrinho Virtual

O código abaixo implementa um cofre virtual simples que permite ao usuário realizar operações básicas de gerenciamento de saldo, como depositar, sacar e verificar o saldo disponível. A estrutura principal do cofre é composta por um saldo, que é representado em centavos. O programa se inicia com a configuração do console e a inicialização do cofre, seguida por uma mensagem de boas-vindas. O usuário é então apresentado a opções interativas por meio de um menu, onde pode escolher entre sacar dinheiro, depositar dinheiro, exibir o saldo atual ou sair do programa. Cada operação é tratada por rotinas específicas, que garantem que o saldo não fique negativo e que os depósitos sejam válidos. O código também inclui verificações de erros para opções inválidas e valores negativos, garantindo uma experiência de uso mais robusta e amigável.

```
O cofrinho é uma estrutura com
   Um número denominado saldo.

Um real é 100 centavos.
Um centavo é um número.
Uma opção é uma string.

Rotina para que se execute o programa:
  Prepare o Console.
  Inicialize o cofrinho.
  Escreva o texto de introdução.
  Exiba as opções do cofrinho.
  Leia uma opção a partir do console.
  Feche o programa.

Rotina para que se inicialize o cofrinho:
  Atribua 0 para o saldo deste cofrinho.

Rotina para que se escreva o texto de introdução:
  Escreva o texto CRLF para StdOut.
  Escreva "Seja bem-vindo ao seu cofrinho virtual." junto com o texto CRLF para StdOut.

Rotina para que se exiba as opções do cofrinho:
  Escreva o texto CRLF para StdOut.
  Escreva "Digite o número correspondente à opção desejada:" junto com o texto CRLF para StdOut.
  Escreva o texto CRLF para StdOut.
  Escreva "1 - Sacar" junto com o texto CRLF para StdOut.
  Escreva "2 - Depositar" junto com o texto CRLF para StdOut.
  Escreva "3 - Exibir Saldo" junto com o texto CRLF para StdOut.
  Escreva "4 - Sair." junto com o texto CRLF para StdOut.
  Escreva o texto CRLF para StdOut.

Rotina para que se leia uma opção a partir do console:
  Leia uma string desde a StdIn.
  Se a string for "1",
    Escreva o texto CRLF para StdOut;
    Retire dinheiro do cofrinho;
    Exiba as opções do cofrinho.
  Se a string for "2",
    Escreva o texto CRLF para StdOut;
    Deposite dinheiro no cofrinho;
    Exiba as opções do cofrinho.
  Se a string for "3",
    Escreva o texto CRLF para StdOut;
    Exiba o saldo do cofrinho;
    Exiba as opções do cofrinho.
  Se a string for "4",
    Retorne.
  Se a string não for alguma opção válida,
    Escreva o texto CRLF para StdOut;
    Escreva "Erro. Opção inválida. Tente Novamente" junto com o texto CRLF para StdOut;
    Exiba as opções do cofrinho.
  Leia a opção a partir do console.

Função para que se determine se uma string é alguma opção válida:
  Se a string for "1", diga sim.
  Se a string for "2", diga sim.
  Se a string for "3", diga sim.
  Se a string for "4", diga sim.
  Diga não.

Rotina para que se retire dinheiro do cofrinho:
  Escreva "Digite a quantidade de centavos que deseja retirar: " para StdOut.
  Leia uma string desde a StdIn.
  Converta a string para um número.
  Se o número for maior do que o saldo deste cofrinho,
    Escreva o texto CRLF para StdOut;
    Escreva "Erro. Saldo Insuficiente no cofrinho." para StdOut;
    Escreva o texto CRLF para StdOut;
    Exiba o saldo do cofrinho;
    Retorne.
  Subtraia o número desde o saldo deste cofrinho.
  Escreva "Fundos retirados com sucesso" junto com o texto CRLF para StdOut.
  Escreva o texto CRLF para StdOut.
  Exiba o saldo do cofrinho.

Rotina para que se deposite dinheiro no cofrinho:
  Escreva "Digite a quantidade de centavos que deseja depositar: " para StdOut.
  Leia uma string desde a StdIn.
  Converta a string para um número.
  Se o número for menor do que 0,
    Escreva "Erro. Valor negativo." para StdOut;
    Escreva o texto CRLF para StdOut;
    Deposite dinheiro no cofrinho.
  Adicione o número ao saldo deste cofrinho.
  Escreva "Fundos adicionados com sucesso" junto com o texto CRLF para StdOut.
  Exiba o saldo do cofrinho.

Rotina para que se exiba o saldo do cofrinho:
  Se o saldo deste cofrinho for menor do que 100,
    Escreva o texto CRLF para StdOut;
    Escreva "O saldo do cofrinho é de " junto com o saldo deste cofrinho junto com " centavos." para StdOut;
    Escreva o texto CRLF para StdOut;
    Retorne.
  Atribua o saldo deste cofrinho dividido por 100 para um número denominado quantidade de reais.
  Atribua a quantidade de reais vezes 100 para um número denominado reais centavizados.
  Atribua o saldo deste cofrinho menos os reais centavizados para um número denominado quantidade de centavos.
  Se a quantidade de centavos for maior do que 9, 
    Escreva o texto CRLF para StdOut;
    Escreva "O saldo do cofrinho é de R$ " junto com a quantidade de reais junto com "," junto com a quantidade de centavos para StdOut.
  Se a quantidade de centavos for menor do que 10, 
    Escreva o texto CRLF para StdOut;
    Escreva "O saldo do cofrinho é de R$ " junto com a quantidade de reais junto com ",0" junto com a quantidade de centavos para StdOut.
  Escreva o texto CRLF para StdOut.
```

