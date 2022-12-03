# Diagrama de Comunicação

## 1. Introdução

O Diagrama de Comunicação, também chamado de Diagrama de Colaboração na versão mais antiga da UML, é um tipo de diagrama de interação dinâmico parecido com um diagrama de sequência, porém mais simplificado com o foco principal em mostrar interações entre objetos e/ou partes usando mensagens sequenciais em um arranjo livre.

Cada objeto é representado como uma linha de vida, que corresponde a um participante individual nas interações, ou seja, representam apenas uma entidade de interação. Caso haja uma conexão multivalorada, a linha de vida deve conter um seletor que especifica qual parte é representada por ela, ou, se omitido, significa que uma representação arbitrária do elemento é escolhida. São representadas por retângulos no diagrama.

Os objetos são representados por retângulo com conectores entre eles que correspondem às associações. As mensagens representam ações e são contidas nessas associações com setas direcionando o fluxo e números que indicam a ordem que são realizadas.

## 2. Metodologia

Os diagramas foram elaborados com base em duas visões, do comprador e do gestor de rifas, enfatizando suas principais interações com sistema e a sequencia que são realizadas. As informações foram abstraidas dos requisitos elicitados em conjunto pela equipe no processo de brainstorm.

A ferramenta utilizada foi o [Lucidchart](https://www.lucidchart.com), que oferece suporte à modelagem de diagramas UML.

## 3. Diagramas de Comunicação

### 3.1 Interação do Comprador

![comunicaçãoCliente](/../../assets/diagComunicacaoCliente.jpeg)

### 3.2 Interação do Gestor de Rifas

![comunicaçãoGestor](/../../assets/diagComunicacaoGestor.jpeg)

## 4. Referências

- **UML Communication Diagrams Overview**. UML Diagrams. Disponível em: https://www.uml-diagrams.org/communication-diagrams.html. Acesso em: 01 dez. 2022.
- **UML 2 Tutorial - Communication Diagram**. SPARX SYSTEMS. Disponível em: https://sparxsystems.com/resources/tutorials/uml2/communication-diagram.html. Acesso em: 03 dez. 2022.
- SERRANO, Milene. **06b - VideoAula - DSW-Modelagem - Comunicacao**. 2020. Acesso em: 03 dez. 2022

## 5. Histórico de Versões

| Data       | Versão | Descrição                               | Autor(es)       |
| ---------- | ------ | --------------------------------------- | --------------- |
| 30/11/2022 | 1.0    | Diagrama de comunicação do cliente - v1 | Karla Feliciano |
| 01/12/2022 | 1.1    | Diagrama de comunicação do gestor - v1  | Karla Feliciano |
| 03/12/2022 | 2.0    | Adição da documentação                  | Karla Feliciano |
