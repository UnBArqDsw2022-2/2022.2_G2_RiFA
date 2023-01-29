# Documento de Arquitetura (DAS)

## Histórico de Versões

| Data  | Versão | Descrição                            | Autor(es) | Revisor(es) |
| ----- | ------ | ------------------------------------ | --------- | ----------- |
| 29-01 | 1.0    | Criação do documento                 | Eurico    | Lucas       |
| 29-01 | 1.1    | Estrutura do documento               | Lucas     | Eurico      |
| 29-01 | 1.2    | Visão de implantação e implementação | Eurico    | Lucas       |

## 1. Introdução

## 2. Representação Arquitetural

### 2.1. Backend

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

### 2.2. Frontend

<center>

![react](../../assets/react-logo.png)

> Figura 3: Logo React. Fonte: https://reactjs.org/ .

</center>

Já para o desenvolvimento da interface visual do projeto, a equipe escolheu fazer o uso da biblioteca de Javascript React. O React é uma biblioteca amplamente utilizada para criar interfaces de usuário interativas de uma maneira mais fácil por atualizar e renderizar componentes automaticamente quando o estado ou os dados do sistema forem alterados. Dessa forma, o React é baseado por componentes, onde cada um destes componentes lida com seu próprio estado e realiza sua própria função, assim diminuindo o acoplamento e aumentando a coesão do sistema. Quando juntos estes componentes passam a compor uma interface gráfica complexa e rica.

Assim como o framework utilizado no backend, a biblioteca React foi escolhida principalmente pela experiência prévia de alguns membros da equipe, que por já terem utilizado-o anteriormente, se sentiram confortáveis não só em desenvolver partes da aplicação, mas também em ensinar outros colegas com menos experiência.

### 2.3. Banco de Dados

<center>

![react](../../assets/postgre-logo.png)

> Figura 4: Logo postgreSQL. Fonte: https://www.postgresql.org/ .

</center>

Para o banco de dados, nós optamos por utilizar o PostgreSQL, que é um sistema gerenciador de banco de dados relacional de código aberto que tem sido amplamente utilizado em projetos devido à sua confiabilidade, escalabilidade e recursos avançados de gerenciamento de dados. Além disso, PostgreSQL é um sistema objeto-relacional, o que significa que ele combina os recursos de um banco de dados relacional tradicional com os de um banco de dados orientado a objetos. Isso significa que ele permite a criação de tipos de objeto personalizados, herança entre objetos e armazenamento de objetos complexos. Somado a isso, ele tem uma ampla comunidade de usuários e contribuidores, o que significa que há uma ampla gama de ferramentas, extensões e recursos disponíveis para ajudar na implementação.

## 3. Metas e Restrições da Arquitetura

## 4. Visão Lógica

## 5. Visão de Implantação

A visão de implantação é uma forma de demonstrar as relações entre os componentes. Abaixo temos um diagrama de implantação, que demonstra quais partes dependem de quais.
![Diagrama de Implantação](docs/assets/diagrama-de-implantacao.png)

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
