---
description: >-
  Muitas vezes iremos precisar desenhar elementos na tela. Este algoritmo cria
  uma espécie de ilusão de ótima ao brincar com as cores.
---

# Desenhando e pintando retângulos e caixas



```
Rotina para que se execute o programa:
  Inicialize os componentes.
  Limpe a tela com a cor preta.
  Exiba a distorção cromática.
  Aguarde pela tecla Esc.
  Feche o programa.

Rotina para que se exiba a distorção cromática:
  Prepare o layout.
  Pinte a malha quadriculada.

Um comprimento é um número.

A largura é um número.
A distância é um número.
O comprimento do quadrado é um número.
A largura da listra é um número.
O número da linha é um número.
O quadrado é uma caixa.
A listra vermelha é uma caixa.
A listra amarela é uma caixa.
A listra azul escuro é uma caixa.
A listra azul claro é uma caixa.

Rotina para que se prepare o layout:
  Atribua a largura desta tela para a largura.
  Atribua a largura dividido por 8 para a distância.
  Atribua a largura dividido por 16 para o comprimento do quadrado.
  Atribua o comprimento do quadrado dividido por 8 para a largura da listra.
  Faça o quadrado [usando] o comprimento do quadrado pelo comprimento do quadrado.
  Faça cada listra usando a largura da listra pelo comprimento do quadrado.
  Posicione todas as caixas no canto superior esquerdo da tela.
  Ajuste o posicionamento inicial das listras.

Rotina para que se faça cada listra usando uma largura por um comprimento:
  Faça a listra vermelha [com] a largura pelo comprimento.
  Faça a listra amarela [com] a largura pelo comprimento.
  Faça a listra azul escuro [com] a largura pelo comprimento.
  Faça a listra azul claro [com] a largura pelo comprimento.

Rotina para que se posicione todas as caixas no canto superior esquerdo da tela:
  Mova o quadrado para o canto superior esquerdo dessa caixa desta tela.
  Mova a listra vermelha para o canto superior esquerdo dessa caixa desta tela.
  Mova a listra amarela para o canto superior esquerdo dessa caixa desta tela.
  Mova a listra azul escuro para o canto superior esquerdo dessa caixa desta tela.
  Mova a listra azul claro para o canto superior esquerdo dessa caixa desta tela.

Rotina para que se ajuste o posicionamento inicial das listras:
  Mova a listra amarela para a direita [usando] a largura da listra.
  Mova a listra azul escuro para a direita [usando] o comprimento do quadrado.
  Mova a listra azul escuro para a esquerda [usando] a largura da listra.
  Mova a listra azul claro para a direita [usando] o comprimento do quadrado.
  Mova a listra azul claro para a esquerda [usando] a largura da listra.
  Mova a listra azul claro para a esquerda [usando] a largura da listra.

Rotina para que se pinte a malha quadriculada:
  Atribua 0 para o número da linha.
  Itere.
    Pinte todas as caixas.
    Mova todas as caixas para a direita usando a distância.
    Atualize a tela.
    Se o quadrado estiver tocando a caixa desta tela, reitere.
    Adicione 1 ao número da linha.
    Mova todas as caixas para a esquerda da tela.
    Mova todas as caixas para baixo usando o comprimento do quadrado.
    Ajuste as listras após descer.
    Se o número da linha for ímpar,
      Mova todas as caixas para a direita usando o comprimento do quadrado.
    Se o quadrado estiver tocando a caixa desta tela, reitere.

Rotina para que se pinte todas as caixas:
  Pinte o quadrado com a cor branca e a cor branca.
  Pinte a listra vermelha com a cor vermelho claro e a cor vermelho claro.
  Pinte a listra amarela com a cor amarela e a cor amarela.
  Pinte a listra azul escuro com a cor azul celeste escuro e a cor azul celeste escuro.
  Pinte a listra azul claro com a cor azul celeste claro e a cor azul celeste claro.

Rotina para que se mova todas as caixas para a direita usando um número:
  Mova o quadrado para a direita [usando] o número.
  Mova a listra vermelha para a direita [usando] o número.
  Mova a listra amarela para a direita [usando] o número.
  Mova a listra azul escuro para a direita [usando] o número.
  Mova a listra azul claro para a direita [usando] o número.

Rotina para que se mova todas as caixas para a esquerda da tela:
  Mova o quadrado para o lado esquerdo dessa caixa desta tela.
  Mova a listra vermelha para o lado esquerdo dessa caixa desta tela.
  Mova a listra amarela para o lado esquerdo dessa caixa desta tela.
  Mova a listra azul escuro para o lado esquerdo dessa caixa desta tela.
  Mova a listra azul claro para o lado esquerdo dessa caixa desta tela.

Rotina para que se mova todas as caixas para baixo usando uma distância:
  Mova o quadrado para baixo [usando] a distância.
  Mova a listra vermelha para baixo [usando] a distância.
  Mova a listra amarela para baixo [usando] a distância.
  Mova a listra azul escuro para baixo [usando] a distância.
  Mova a listra azul claro para baixo [usando] a distância.

Rotina para que se ajuste as listras após descer:
  Mova a listra amarela para a direita [usando] a largura da listra.
  Mova a listra azul escuro para a direita [usando] o comprimento do quadrado.
  Mova a listra azul escuro para a esquerda [usando] a largura da listra.
  Mova a listra azul claro para a direita [usando] o comprimento do quadrado.
  Mova a listra azul claro para a esquerda [usando] a largura da listra.
  Mova a listra azul claro para a esquerda [usando] a largura da listra.

```

<figure><img src="../.gitbook/assets/distorção cromática.png" alt=""><figcaption><p>Resultado da execução do programa</p></figcaption></figure>
