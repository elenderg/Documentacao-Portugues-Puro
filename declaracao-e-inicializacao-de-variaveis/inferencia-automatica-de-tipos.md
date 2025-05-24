# Inferência automática de tipos

O compilador é capaz de identificar automaticamente o tipo de uma variável, com base no nome dela.

Exemplo:

```
Atribua "João" para uma nova string.
```

Ao se deparar com a linha acima, o compilador executa as seguintes ações:

1. Cria uma variável local denominada "nova string".
2. A partir do nome da variável, infere seu tipo (string, neste caso).
3. Inicializa  a variável "nova string" com o valor "João".

À primeira vista pode parecer que a string literal "João" foi o que ajudou o compilador a detectar o tipo da variável. Porém não é este o caso. Veja o exemplo abaixo:

```
Um par de números fracionários é uma estrutura com
  Uma fração e
  Uma segunda fração.
```

Embora o tipo "segunda fração" não esteja definido em lugar algum, o compilador irá, a partir do nome da variável inferir seu tipo corretamente como "fração".
