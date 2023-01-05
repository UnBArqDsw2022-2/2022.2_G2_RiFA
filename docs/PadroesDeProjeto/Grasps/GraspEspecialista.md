# GRASP Foco: Especialista

## Histórico de Versões

| Data   | Versão | Descrição                | Autor(es)    | Revisor(es) |
| ------ | ------ | ------------------------ | ------------ | ----------- |
| 05-Jan | 0.1    | Criação do documento     | Eurico Abreu | -           |
| 05-Jan | 0.2    | Introdução               | Eurico Abreu | -           |
| 05-Jan | 0.3    | Finalização do documento | Eurico Abreu | -           |

## 1. Introdução

O padrão GRASP especialista tem a sua preocupação principal em atribuir responsabilidades para a entidade mais especialista em um dado aspecto, não apenas na criação de instâncias, mas em todos os aspectos do sistema. Tem bastante semelhança com o GRASP Criador, já que todo criador é um especialista em criar instâncias.
A utilização desse padrão GRASP tem algumas consequências, por exemplo:

- Alta coesão, devido ao fato que os objetos fazem tudo relacionados a suas informações.
- Encapsulação, já que os objetos usam as suas próprias informações para realizar as suas tarefas.
- Baixo acoplamento, gerando sistemas mais fáceis de manter.

## 2. Aplicação no projeto

Em nosso projeto, encontramos um exemplo de GRASP especialista no diagrama de classes de entidades, no caso escolhido, a classe Produto é a especialista. Como mostra a imagem a baixo.

<center>

![Imagem](../../assets/graspsEspecialista.png)

Figura 1 -> Fonte: Diagrama de classes

</center>

## 3. Conclusão

Para concluir, podemos dizer que as vantagens de se usar o padrão GRASP Especialista são bastantes expressivas. Aumentamos a coesão, diminuimos o acoplamento e aumentamos o encapsulamento, isso tudo isso facilita a evolução do software.

## Referências

- [1] SERRANO, Milene. Arquitetura e Desenho de Software. AULA - GRASP – PARTE I e II. Acesso em: 04 jan. 2023.
- [2] SERRANO, Milene. Arquitetura e Desenho de Software. AULA - GRASP – COMPLEMENTAR A e B. Acesso em: 04 jan. 2023.
- [3] Basseto, Nelson. RDD – Responsibility Driven Design e GRASP – General Responsibility Assignment Software Principles. Disponivel em: http://nelsonbassetto.com/blog/tags/grasp/ Acesso em: 04 jan. 2023.
