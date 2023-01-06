# Composite

## Histórico de Versões

| Data   | Versão | Descrição                       | Autor(es)      |
| ------ | ------ | ------------------------------- | -------------- |
| 05-Jan | 0.1    | Construção da Página            | Jackes Fonseca |
| 05-Jan | 0.2    | Adiciona introdução             | Jackes Fonseca |
| 05-Jan | 0.3    | Adiciona aplicação e introdução | Jackes Fonseca |

## 1. Introdução

O Composite é um padrão de projeto estrutural que permite que você componha objetos em estruturas de árvores e então trabalhe com essas estruturas como se elas fossem objetos individuais.

## 2. Metodologia

Usar o padrão Composite faz sentido apenas quando o modelo central de sua aplicação pode ser representada como uma árvore. O padrão Composite sugere que você trabalhe com Produtos e Caixas através de uma interface comum que declara um método para a contagem do preço total.

Para um produto, ele simplesmente retornaria o preço dele. Para uma caixa, ele teria que ver cada item que ela contém, perguntar seu preço e então retornar o total para essa caixa. Se um desses itens for uma caixa menor, aquela caixa também deve verificar seu conteúdo e assim em diante, até que o preço de todos os componentes internos sejam calculados. Uma caixa pode até adicionar um custo extra para o preço final, como um preço de embalagem.

<figure>
  <figcaption style="text-align: center !important">
    Figura 1: Diagrama do GoF de Composite
  </figcaption>

  <div style="background-color:#000">

  ![Diagrama de Classes - Interfaces](https://user-images.githubusercontent.com/53023400/210824670-121c6f87-b86f-4e03-986f-d0d3561e1d90.png)

  </div>

  <figcaption style="text-align: center !important">
    Fonte: <a href="https://refactoring.guru/pt-br/design-patterns/composite">Design Patterns</a>
  </figcaption>
</figure>

## 3. Exemplos no código

Conforme o diagrama de componentes abaixo, foi feita uma sugestão de utilização do padrão composite para o escopo de rifas usando o sistema de carrinho de compras.

<figure>
  <figcaption style="text-align: center !important">
    Figura 2: Diagrama de componentes
  </figcaption>

  ![carrinho-compras](https://user-images.githubusercontent.com/53023400/210902718-04109e26-2c1b-4460-b89f-56bdbe4886c7.png)

  <figcaption style="text-align: center !important">
    Fonte: Próprio autor
  </figcaption>
</figure>


<figure>
  <figcaption style="text-align: center !important">
    Figura 3: Rifa Componente (Interface)
  </figcaption>

  ![rifa-component](https://user-images.githubusercontent.com/53023400/210902779-5704171c-04a9-448c-8508-85c112369101.png)

  <figcaption style="text-align: center !important">
    Fonte: Próprio autor
  </figcaption>
</figure>


<figure>
  <figcaption style="text-align: center !important">
    Figura 4: Produto
  </figcaption>

  <div style="background-color:#000">

  ![produto](https://user-images.githubusercontent.com/53023400/210902908-91eb3ac5-a14b-4a06-a308-4f7e80ac50ba.png)

  </div>

  <figcaption style="text-align: center !important">
    Fonte: Próprio autor
  </figcaption>
</figure>

<figure>
  <figcaption style="text-align: center !important">
    Figura 5: Rifa (Leaf)
  </figcaption>

  <div style="background-color:#000">

  ![rifa](https://user-images.githubusercontent.com/53023400/210903001-8a9f5287-aacc-4c13-ab31-dff76544cbf3.png)

  </div>

  <figcaption style="text-align: center !important">
    Fonte: Próprio autor
  </figcaption>
</figure>


<figure>
  <figcaption style="text-align: center !important">
    Figura 6: Pedido (leaf)
  </figcaption>

  <div style="background-color:#000">

  ![pedido](https://user-images.githubusercontent.com/53023400/210904194-f296fba9-bb5e-49e9-8511-4008f347e35f.png)

  </div>

  <figcaption style="text-align: center !important">
    Fonte: Próprio autor
  </figcaption>
</figure>

<figure>
  <figcaption style="text-align: center !important">
    Figura 6: Rifa composite (Composite)
  </figcaption>

  <div style="background-color:#000">

  ![rifa-composite](https://user-images.githubusercontent.com/53023400/210904378-7b90846f-4f0f-4172-ac50-f7d82bcc6a88.png)

  </div>

  <figcaption style="text-align: center !important">
    Fonte: Próprio autor
  </figcaption>
</figure>

## 4. Conclusão
O maior benefício dessa abordagem é que você não precisa se preocupar sobre as classes concretas dos objetos que compõem essa árvore. Você não precisa saber se um objeto é um produto simples ou uma caixa sofisticada. Você pode tratar todos eles com a mesma interface. Quando você chama um método os próprios objetos passam o pedido pela árvore.

## 5. Bibliografia
> [1] Composite. Disponível em: <https://refactoring.guru/pt-br/design-patterns/composite>. Acesso em: 22 de novembro de 2022.
