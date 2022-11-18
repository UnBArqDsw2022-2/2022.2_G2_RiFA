# Metodolia Adotada

### Participantes do Artefato

- Guilherme Brito

### 1. Introdução

Este documento tem por objetivo apresentar e descrever todas as metodologias adotadas durante o ciclo de desenvolvimento
do Projeto, seja desde a fase de concepção à sua implementação. Aqui serão descritos os métodos e ferramentas adotadas.

### 2. Metodologias Adotadas

Após uma reunião realizada no dia 11 de Novembro com a presença da maioria dos membros decidiu-se pela utilização de uma
metodologia mista utilizando de conceitos advindos de **Metodologias Ágeis**.
A escolha se deu devido à familiaridade do grupo com essas técnicas que serão descritas abaixo.

#### 2.1 - Kanban Board

Kanban é um sistema visual de gestão de trabalho, que busca conduzir cada tarefa por um fluxo predeterminado de
trabalho.[1]
Em geral, o conceito de Kanban pode ser definido pelos seguintes itens:

- O sistema **visual**: um processo, definido em um quadro com colunas de separação, que permite dividir o trabalho em
  segmentos ou pelo seu status.
- Cartões: Descrevem o trabalho real que transita por este processo.

Neste trabalho utilizamos da ferramenta Github que apresenta a funcionalidade Projects. Nela, podemos construir
visualizações tomando Issues como Base.

O quadro foi construído tomando as colunas mais comuns utilizadas como base e pode ser visualizado na figura abaixo.

|   ![Imagem](../../assets/kanban-board.png)   |
|:--------------------------------------------:|
| Figura 1 : Kanban Board Utilizado no Projeto |

As colunas se caracterizam em:

- **Todo**: Issues que são identificadas, mas que não foram iniciadas.
- **In Progress**: Issues que foram atribuídas a algum participante e estão em desenvolvimento.
- **Under Review**: Issues que estão aguardando uma revisão.
- **Done**: Issues finalizadas e que já estão no ambiente de Produção.

#### 2.2 - Scrum

O Scrum trata-se de um método de trabalho realizado a partir de pequenos ciclos de atividades dentro de um projeto.

Foram utilizados as seguintes técnicas advindas dessa metodologia:

- **Sprint**: Um período de tempo predefinido em que as tarefas devem ser realizadas pela equipe. Neste projeto, cada
  Sprint
  terá por duração entre 7 a 10 dias, a depender de diversos fatores, como: Complexidade da Entrega, disponibilidade dos
  participantes, etc.
- **Product Backlog**: Desmembramento da Visão do Produto em funcionalidades (que em união à utilização do Kanban
  Boards,
  essas funcionalidades se tornam Cartões). No contexto do projeto, o Kanban Board servirá de apoio para esse backlog.
    - Importante salientar que o Backlog será restrito a milestone atual (prazos definidos no plano de ensino da
      disciplina).
- **Spring Planning**: Evento de planejamento onde serão definidas as tarefas que serão implementadas na Sprint atual.
    - Como todo o planejamento das entregas (definido no plano de ensino disponível no Aprender3) já é de conhecimento
      de toda a equipe, no contexto do projeto esse conceito será utilizado na organização de reuniões para que as
      tarefas possam ser atribuídas.
- **Sprint Reviews**: Evento de revisões de Sprints onde os participantes apresentam o trabalho realizado durante a
  Sprint.
  No Contexto do Projeto, também foi utilizado do conceito de Pull Requests, onde a cada funcionalidade criada ou
  melhoria realizada, o autor "abre" um Pull Request solicitando o "merge" de sua funcionalidade (produzida em uma
  Branch separada) ao ambiente de produção (possuindo uma Branch dedicada a isso). Um outro participante do grupo irá
  ser responsável pela Validação e Verificação dessa *nova feature*.

### Ferramentas Utilizadas

Para a facilitação da execução do processo, foram utilizadas as ferramentas descritas na tabela abaixo.

| Nome da Ferramenta |                                                 Objetivo do Uso da Ferramenta                                                  |
|:------------------:|:------------------------------------------------------------------------------------------------------------------------------:|
|       Github       |                                   Fins de versionamento, planejamento e gerência de Tarefas.                                   |
|      Whatsapp      |                                      Comunicação da equipe com uso de mensagens diárias.                                       |
|       Teams        |                            Gravação de Reuniões e Sessões de Brainstorming realizadas pela equipe.                             |
|      Discord       |                                                      Reuniões da equipe.                                                       |
|  Camunda Modeler   |                                          Desenho dos processos e dos diagramas BPMNs.                                          |
|     LucidChart     |                                                    Modelagem dos diagramas.                                                    |
|   IntelliJ IDEA    | IDE utilizada em todo o processo de produção do Trabalho, desde construção da Wiki em Arquivos .md até a produção dos códigos. |

## Referências

- [1] - **O que é Kanban?** Disponível em: https://www.totvs.com/blog/negocios/kanban/

## Histórico de Versões

| Data   | Versão | Descrição            | Autor(es)       |
|--------|--------|----------------------|-----------------|
| 16-Nov | 0.1    | Construção da Página | Guilherme Brito |

