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
