---
description: >-
  Uma agenda telefônica permite armazenar e organizar informações de contato de
  pessoas e empresas. Este algoritmo implementa uma agenda simples, usando
  listas duplamente encadeadas.
---

# Agenda Telefônica

{% code overflow="wrap" %}
```
Um contato é uma lista com
  Uma string denominada nome e
  Uma string denominada número de telefone.

A agenda telefônica é [composta de] uns contatos.

O comando é um trecho.

Rotina para que se execute o programa:
  Defina "console" como o tipo da aplicação.
  Escreva o texto CRLF junto com "Digite um comando: " para StdOut.
  Itere.
    Escreva o texto CRLF junto com " > " para StdOut.
    Leia o comando desde a StdIn.
    Se o comando estiver em branco,
      Reitere.
    Se o comando for "adicionar", 
      Adicione o contato;
      Reitere.
    Se o comando for "alterar", 
      Altere o contato;
      Reitere.
    Se o comando for "mudar", 
      Altere o contato;
      Reitere.
    Se o comando for "apagar", 
      Exclua o contato;
      Reitere.
    Se o comando for "excluir", 
      Exclua o contato;
      Reitere.
    Se o comando for "encontrar", 
      Encontre o contato;
      Reitere.
    Se o comando for "ajuda", 
      Mostre o menu de ajuda;
      Reitere.
    Se o comando for "listar", 
      Liste os contatos;
      Reitere.
    Se o comando for "fechar", 
      Destrua a agenda telefônica;
      Pare.
    Se o comando for "sair",
      Destrua a agenda telefônica;
      Pare.
  Reitere.
  Feche o nosso programa.

Rotina para que se mostre o menu de ajuda:
  Escreva o texto CRLF junto com "Comandos Disponíveis:" para StdOut.
  Escreva o texto CRLF junto com "Adicionar" para StdOut.
  Escreva o texto CRLF junto com "Alterar" para StdOut.
  Escreva o texto CRLF junto com "Excluir" para StdOut.
  Escreva o texto CRLF junto com "Encontrar" para StdOut.
  Escreva o texto CRLF junto com "Listar" para StdOut.
  Escreva o texto CRLF junto com "Sair" para StdOut.
  Escreva o texto CRLF junto com "Adicionar" para StdOut.

Rotina para que se adicione o contato:
  Aloque memória para um contato.
  Acrescente o contato na agenda telefônica.
  Escreva "Digite o nome do contato: " junto com o texto CRLF para StdOut.
  Leia uma string desde a StdIn.
  Atribua a string para o nome deste contato.
  Escreva "Digite o telefone do contato: " junto com o texto CRLF para StdOut.
  Leia uma nova string desde a StdIn.
  Atribua a nova string para o número de telefone deste contato.
  Escreva "Contato adicionado." junto com o texto CRLF para StdOut.

Rotina para que se altere o contato:
  Escreva "Digite o nome do contato a ser alterado: " junto com o texto CRLF para StdOut.
  Leia uma string denominada nome desde a StdIn.
  Encontre um contato usando o nome.
  Se o contato for inexistente,
    Escreva "Contato não encontrado." junto com o texto CRLF para StdOut;
    Retorne.  
  Leia uma string denominada telefone desde a StdIn.
  Atribua o telefone para o número de telefone deste contato.
  Escreva "Contato alterado." junto com o texto CRLF para StdOut.

Rotina para que se exclua o contato:
  Escreva "Digite o nome do contato a ser excluído: " junto com o texto CRLF para StdOut.
  Leia uma string denominada nome desde a StdIn.
  Encontre um contato usando o nome.
  Se o contato for inexistente,
    Escreva "Contato não encontrado." junto com o texto CRLF para StdOut;
    Retorne.  
  Remova o contato desde a agenda telefônica.
  Destrua o contato.
  Escreva "Contato excluído." junto com o texto CRLF para StdOut.

Rotina para que se encontre o contato:
  Escreva "Digite o nome do contato a ser encontrado: " junto com o texto CRLF para StdOut.
  Leia uma string denominada nome desde a StdIn.
  Encontre um contato usando o nome.
  Se o contato for inexistente,
    Escreva "Contato não encontrado." junto com o texto CRLF para StdOut;
    Retorne.  
  Escreva o nome deste contato junto com a tabulação horizontal junto com "            " junto com o número de telefone deste contato junto com o texto CRLF para StdOut.

Rotina para que se liste os contatos:
  Itere.
    Obtenha um contato desde a agenda telefônica.
    Se o contato for inexistente, pare.
    Escreva o nome deste contato junto com a tabulação horizontal junto com "            " junto com o número de telefone deste contato junto com o texto CRLF para StdOut.
  Reitere.
  Se a contagem desta agenda telefônica for igual a 1,
    Atribua a contagem desta agenda telefônica junto com " contato." para uma string.
  Se a contagem desta agenda telefônica for maior do que 1,
    Atribua a contagem desta agenda telefônica junto com " contatos." para a string.
  Escreva o texto CRLF junto com a string junto com o texto CRLF para StdOut.

Rotina para que se encontre um contato usando uma string:
  Atribua inexistente para o contato.
  Itere.
    Obtenha o contato desde a agenda telefônica.
    Se o contato for inexistente, pare.
    Se o nome deste contato começar com a string, pare.
  Reitere.
```
{% endcode %}
