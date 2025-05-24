# Lidando com vazamentos de memória em laços

Por convenção, usamos os verbos "criar" e "destruir" sempre que alocação e desalocação de memória dinâmica estiverem envolvidas. É sua responsabilidade destruir o que quer que você criar antes de encerrar o seu programa. Se não fizer isso, você causará um "vazamento de memória", parecido com o da imagem abaixo:

<figure><img src="../.gitbook/assets/Elementos no Heap.PNG" alt=""><figcaption></figcaption></figure>

Eis o código que gerou este aviso. Leia-o e tente identificar o erro:

{% code lineNumbers="true" %}
```
Rotina para que se execute o programa:
  Carregue as bibliotecas padrão do sistema.
  Limpe a tela.
  Mostre a seta do mouse.
  Faça uma caixa 96 px por 48 px.
  Centralize a caixa sobre a tela.
  Itere.
    Desenfileire um evento.
    Se o evento for inexistente, pare.
    Se a categoria deste evento for "movimentação de cursor", 
      Execute o evento usando a caixa (exibir cursor do mouse).
    Se a categoria deste evento for "clique do botão esquerdo",
      Retorne.
  Reitere.
  Desmanche todos os eventos.
  Feche o programa.

Rotina para que se execute um evento usando uma caixa (exibir cursor do mouse):
  Atribua a cor branca a uma cor.
  Se a localização deste evento estiver na caixa, 
    Atribua a cor verde à cor.
  Pinte e preencha a caixa com a cor.
  Atualize a tela.
```
{% endcode %}



É um detalhe ínfimo, mas comum. Olhe para o código corrigido:

{% code lineNumbers="true" %}
```
Rotina para que se execute o programa:
  Carregue as bibliotecas padrão do sistema.
  Limpe a tela.
  Mostre a seta do mouse.
  Faça uma caixa 96 px por 48 px.
  Centralize a caixa sobre a tela.
  Itere.
    Desenfileire um evento.
    Se o evento for inexistente, pare.
    Se a categoria deste evento for "movimentação de cursor", 
      Execute o evento usando a caixa (exibir cursor do mouse).
    Se a categoria deste evento for "clique do botão esquerdo",
      Pare.
  Reitere.
  Desmanche todos os eventos.
  Feche o programa.

Rotina para que se execute um evento usando uma caixa (exibir cursor do mouse):
  Atribua a cor branca a uma cor.
  Se a localização deste evento estiver na caixa, 
    Atribua a cor verde à cor.
  Pinte e preencha a caixa com a cor.
  Atualize a tela.
```
{% endcode %}

Perceba que a ÚNICA diferença é a linha 13, onde ao invés de "Pare", o código problemático contém a instrução "Retorne". Caso você utilize a instrução "Retorne" dentro da função Main, acabará encerrando o programa antes de efetuar a desalocação (linhas 19 e 20). Isso ocorre porque a instrução "Retorne" equivale a um "return;" de outras linguagens de programação.
