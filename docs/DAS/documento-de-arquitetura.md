# Documento de Arquitetura (DAS)

## Histórico de Versões

| Data  | Versão | Descrição                            | Autor(es) | Revisor(es) |
| ----- | ------ | ------------------------------------ | --------- | ----------- |
| 29-01 | 1.0    | Criação do documento                 | Eurico    | Lucas       |
| 29-01 | 1.1    | Estrutura do documento               | Lucas     | Eurico      |
| 29-01 | 1.2    | Visão de implantação e implementação | Eurico    | Lucas       |
| 29-01 | 1.3    | Representação arquitetural           | Lucas     | Eurico      |
| 29-01 | 1.4    | Introdução e Visão Lógica            | Karla     |             |
| 30-01 | 1.5    | Metas e Restrições da Arquitetura    | Lucas     | Eurico      |

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

## 3. Representação Arquitetural

### 3.1. Backend

<center>

![Spring Boot](../../assets/Spring-Logo.png)

> Figura 1: Logo Spring. Fonte: https://spring.io .

</center>

Para o desenvolvimento da backend da aplicação, optamos por utilizar Java com o framework Spring Boot. Sendo assim, o Spring Boot é uma parte especializada do Spring Framework, que por sua vez é um framework que oferece uma programação e um modelo de configuração mais compreensivo para aplicações Java. A escolha da equipe em relação ao Spring Boot se deu em parte pela experência prévia de alguns membros com a configuração do ambiente e denvolvimento de aplicações com o framework e, também, pelo framework permitir o desenvolvimento de aplicações de alta qualidade com menores esforços de configuração e deploy.

No quesito arquitetural, o Spring Boot consiste de 4 camadas: Camada de Apresentação, Camada de Negócio, Camada de Persistência e Camada de Dados. Estas camadas se relacionam da seguinte maneira:

<center>

![Arquitetura Spring Boot](../../assets/Spring_Boot-Flow.png)

> Figura 2: Relacionamento entre camadas Spring Boot. Fonte: https://spring.io .

</center>

### 3.2. Frontend

<center>

![react](../../assets/react-logo.png)

> Figura 3: Logo React. Fonte: https://reactjs.org/ .

</center>

Já para o desenvolvimento da interface visual do projeto, a equipe escolheu fazer o uso da biblioteca de Javascript React. O React é uma biblioteca amplamente utilizada para criar interfaces de usuário interativas de uma maneira mais fácil por atualizar e renderizar componentes automaticamente quando o estado ou os dados do sistema forem alterados. Dessa forma, o React é baseado por componentes, onde cada um destes componentes lida com seu próprio estado e realiza sua própria função, assim diminuindo o acoplamento e aumentando a coesão do sistema. Quando juntos estes componentes passam a compor uma interface gráfica complexa e rica.

Assim como o framework utilizado no backend, a biblioteca React foi escolhida principalmente pela experiência prévia de alguns membros da equipe, que por já terem utilizado-o anteriormente, se sentiram confortáveis não só em desenvolver partes da aplicação, mas também em ensinar outros colegas com menos experiência.

### 3.3. Banco de Dados

<center>

![react](../../assets/postgre-logo.png)

> Figura 4: Logo postgreSQL. Fonte: https://www.postgresql.org/ .

</center>

Para o banco de dados, nós optamos por utilizar o PostgreSQL, que é um sistema gerenciador de banco de dados relacional de código aberto que tem sido amplamente utilizado em projetos devido à sua confiabilidade, escalabilidade e recursos avançados de gerenciamento de dados. Além disso, PostgreSQL é um sistema objeto-relacional, o que significa que ele combina os recursos de um banco de dados relacional tradicional com os de um banco de dados orientado a objetos. Isso significa que ele permite a criação de tipos de objeto personalizados, herança entre objetos e armazenamento de objetos complexos. Somado a isso, ele tem uma ampla comunidade de usuários e contribuidores, o que significa que há uma ampla gama de ferramentas, extensões e recursos disponíveis para ajudar na implementação.

## 4. Metas e Restrições da Arquitetura

### 4.1. Metas

- <b>Usabilidade:</b> A interface do aplicativo deve ser intuitiva e fácil de ser utilizada.
- <b>Escalabilidade:</b> O código deve estar estruturado de forma com que permita futuras evoluções.
- <b>Manutenibilidade:</b> O código da aplicação deve permitir manutenção e melhorias que não custem tempo e esforço acima do normal.
- <b>Segurança:</b> A aplicação deverá manter os dados confidenciais de seus usuários armazenados em segurança por meio de ferramentas de encriptação de dados.
- <b>Portabilidade:</b> A aplicação deverá operar com desempenho similar em todos os navegadores que suportar.

### 4.2. Restrições

- <b>Idioma:</b> A aplicação deverá ser desenvolvido no idioma português do Brasil.
- <b>Conectividade:</b> É necessário estar conectado a internet para utilizar a aplicação.
- <b>Plataforma:</b> A aplicação deverá ter suporte para os browsers Chrome, Safari e Firefox.
- <b>Tecnologia:</b> A aplicação será desenvolvida utilizando o framework Java Spring boot e a biblioteca TypeScript React.
- <b>Prazo:</b> A aplicação com as funcionalidades propostas deverá ser finalizada até o dia 30/01/2023

## 5. Visão de Implantação

A visão de implantação é uma forma de demonstrar as relações entre os componentes. Abaixo temos um diagrama de implantação, que demonstra quais partes dependem de quais.

![Diagrama de Implantação](../assets/diagrama-de-implantacao.png)

> Figura 5: Diagrama de Implantação. Autor: Eurico Abreu.

## 6. Visão de Implementação

A visão de implementação tem o foco principal em mostrar como o sistema foi desenvolvido e organizado. Para demonstrar esse tópico podemos usar o Diagrama de Componentes.

### 6.1. Diagrama de componentes

O seguinte diagrama já se encontra no nosso repositório e pode ser encontrado em: [Diagrama de Componentes](docs/Modelagem/diagrama-componentes.md)

<center><iframe height="600" width="700" src="https://github.com/UnBArqDsw2022-2/2022.2_G2_RiFA/blob/main/docs/Modelagem/diagrama-componentes.md#diagrama-de-componentes"></iframe>
</center>

## 7. Visões de Caso de Uso

## 8. Visão de Processos

## 9. Visão de Dados

## 10. Tamanho e Performance

## 11. Qualidade

## Referências

- Spring Boot – Architecture. Disponível em https://www.geeksforgeeks.org/spring-boot-architecture/ Acesso em 29 de janeiro de 2023.
- Documentação React. Disponível em https://reactjs.org/ Acesso em 29 de janeiro de 2023.
- Spring Boot Architecture – Detailed Explanation. Disponível em https://www.interviewbit.com/blog/spring-boot-architecture/ Acesso em 29 de janeiro de 2023.
