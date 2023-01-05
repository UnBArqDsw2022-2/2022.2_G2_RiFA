# Alta Coesão

## Histórico de Versões

| Data   | Versão | Descrição                                  | Autor(es)    | Revisor(es) |
| ------ | ------ | ------------------------------------------ | ------------ | ----------- |
| 04-Jan | 0.1    | Criação do documento                       | Erick Melo   | -           |

## 1. Introdução

O padrão de alta coesão se refere a uma classe ou módulo que tem um conjunto focado de responsabilidades e que trabalha de forma independente, sem depender de outras classes ou módulos para realizar sua função. Isso significa que a classe ou módulo tem um propósito claro e específico, e que todas as suas operações e funcionalidades estão relacionadas a esse propósito.

Um dos principais benefícios da alta coesão é que ela torna o código mais fácil de entender e manter, já que as responsabilidades de cada classe ou módulo são bem definidas e não há sobreposição ou ambiguidade. Além disso, a alta coesão também pode levar a uma maior reutilização do código, já que as classes ou módulos bem definidos podem ser facilmente reutilizados em outros contextos.

## 2. Aplicação

Em nosso projeto, é possível notar um exemplo de alta coesão na classe "Foto" do [diagrama de classes](https://unbarqdsw2022-2.github.io/2022.2_G2_RiFA/#/Modelagem/diagrama_classes), como mostrado abaixo, que possui atributos e métodos relacionados exclusivamente com o escopo da classe. Com essa focalização será possível utilizar essa classe tanto para fotos do produto quanto para fotos do usuário.

<center>
<img src="https://user-images.githubusercontent.com/48844857/210676285-45109b8d-aee4-44de-8c4b-d57fd5996afb.png">
</center>

# 3. Conclusão

Ao utilizarmos o padrão GRASP de alta coesão em nosso projeto, conseguimos criar classes e módulos bem definidos e concentrados em suas responsabilidades específicas. Isso nos permitirá ter um código mais claro e fácil de entender, além de facilitar a manutenção e a reutilização do código em outros contextos caso necessário.

## 4. Referências

> SERRANO, Milene. Arquitetura e Desenho de Software. AULA - GRASP_A - COMPLEMENTAR. Acesso em: 04 jan. 2023.