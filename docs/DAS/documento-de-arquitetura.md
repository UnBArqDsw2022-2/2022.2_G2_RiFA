# Documento de Arquitetura (DAS)

## Histórico de Versões

| Data  | Versão | Descrição                            | Autor(es) | Revisor(es) |
| ----- | ------ | ------------------------------------ | --------- | ----------- |
| 29-01 | 1.0    | Criação do documento                 | Eurico    | Lucas       |
| 29-01 | 1.1    | Estrutura do documento               | Lucas     | Eurico      |
| 29-01 | 1.2    | Visão de implantação e implementação | Eurico    | Lucas       |
| 29-01 | 1.3    | Introdução e Visão Lógica            | Karla     | João Paulo  |

## 1. Introdução

### 1.1 Propósito

Esse documento apresenta uma visão geral da arquitetura do sistema E-Rifas, utilizando diferentes visões arquiteturais para retratar os diferentes aspectos do sistema. A intenção é capturar e transmitir as decisões de arquitetura significativas que foram feitas durante o processo de construção do sistema.

A utilização deste documento pode ser feita tanto por usuários, caso queiram entender melhor o funcionamento do sistema e consultar informações em um só lugar, quanto para os desenvolvedores, que precisarão seguir os padrões e modelos estabelecidos aqui para desenvolver o sistema de forma uniforme.

### 1.2 Escopo

O E-Rifas é um sistema que visa facilitar a compra e venda de rifas online. É possível para um vendedor anunciar diversos produtos que são vendidos através de bilhetes de rifa, e ao final sorteado para um ganhador. E para o comprador, é possível encontrar diversos tipos de rifas em um lugar, e filtrar de acordo com seus interesses.

O Documento de Arquitetura descreve como é projetada a estrutura desse sistema, reunindo informações em tipos de visões, assim como a representação arquitetural e aspectos como tamanho, performance e qualidade, o que facilita a manutenção e desenvolvimento do sistema.

### 1.3 Definições, Acrônimos e Abreviações

Os termos, definições, acrônimos e abreviações necessários para entender e interpretar o projeto e o documento devidamente pode ser encontrado no documento de **[Léxicos](Base/artefatos-design-sprint/lexicos.md)**, realizado na fase Base do desenvolvimento do projeto.

### 1.4 Visão Geral

Para facilitar o entendimento, o documento de arquitetura é dividido da seguinte forma:

- [Visão Lógica](#_2-visão-lógica): descreve as partes arquiteturais significantes dos modelos de design.
- [Visão de Implantação](#_3-visão-de-implantação): descreve as configurações físicas (hardware).
- [Visão de Implementação](#_4-visão-de-implementação): descreve a estrutura geral do modelo de implementação.
- [Visão de Casos de Uso](#_5-visões-de-caso-de-uso): lista os casos de uso ou cenários das funcionalidades do sistema.
- [Visão de Processos](#_6-visão-de-processos): descreve a decomposição do sistema em processos leves ou pesados.
- [Visão de Dados](#_7-visão-de-dados): descreve a camada de persistência do sistema.
- [Representação Arquitetural](#_8-representação-arquitetural): descreve a arquitetura de software do sistema e como é representado.
- [Metas e Restrições da Arquitetura](#_9-metas-e-restrições-da-arquitetura): descreve os objetivos e requisitos do software.
- [Tamanho e Performance](#_10-tamanho-e-performance): descreve as características de dimensão do software.
- [Qualidade](#_11-qualidade): descreve como a arquitetura de software contribui para todas as capacidades do sistema.

## 2. Visão Lógica

A Visão Lógica descreve as partes significantes do modelo de design e mostra as decomposições em subsistemas e pacotes e classes da arquitetura do sistema. Essa visão pode ser representada pelos Diagrama de Pacotes e Diagrama de Classes.

### Diagrama de Pacotes

O diagrama de pacotes é um diagrama UML estrutural e estático que mostra a organização e disposição de um determinado sistema à nível de pacotes.

Esse diagrama foi desenvolvido em outras etapas do projeto e pode ser encontrado em mais detalhes em: [Diagrama de Classes](Modelagem/diagramaPacotes.md).

![pacotesBack](../assets/diagramaPacotesBackEnd.png)

<center>

**Figura 1: Diagrama de Pacotes do Backend**  
Autor: Lucas Pimentel

</center>

![pacotesFront](../assets/diagramaPacotesFrontEnd.png)

<center>

**Figura X: Diagrama de Pacotes do Frontend**  
Autor: Lucas Pimentel

</center>

### Diagrama de Classes

Os Diagramas de classes estão entre os tipos mais úteis de diagramas UML pois mapeiam de forma clara a estrutura de um determinado sistema ao modelar suas classes, seus atributos, operações e relações entre objetos.

Esse diagrama foi desenvolvido em outras etapas do projeto e pode ser encontrado em mais detalhes em: [Diagrama de Pacotes](Modelagem/diagrama_classes.md).

![classes](../assets/uml_classes_ent.png)

<center>

**Figura X: Diagrama de Classes**  
Autor: Guilherme Brito

</center>

## 3. Visão de Implantação

A visão de implantação é uma forma de demonstrar as relações entre os componentes. Abaixo temos um diagrama de implantação, que demonstra quais partes dependem de quais.

![Diagrama de Implantação](../assets/diagrama-de-implantacao.png)

> Figura 1: Diagrama de Implantação. Autor: Eurico Abreu.

## 4. Visão de Implementação

A visão de implementação tem o foco principal em mostrar como o sistema foi desenvolvido e organizado. Para demonstrar esse tópico podemos usar o Diagrama de Componentes.

### 4.1. Diagrama de componentes

O seguinte diagrama já se encontra no nosso repositório e pode ser encontrado em: [Diagrama de Componentes](docs/Modelagem/diagrama-componentes.md)

<center><iframe height="600" width="700" src="https://github.com/UnBArqDsw2022-2/2022.2_G2_RiFA/blob/main/docs/Modelagem/diagrama-componentes.md#diagrama-de-componentes"></iframe>
</center>

## 5. Visões de Caso de Uso

## 6. Visão de Processos

## 7. Visão de Dados

## 8. Representação Arquitetural

## 9. Metas e Restrições da Arquitetura

## 10. Tamanho e Performance

## 11. Qualidade

## Referências
