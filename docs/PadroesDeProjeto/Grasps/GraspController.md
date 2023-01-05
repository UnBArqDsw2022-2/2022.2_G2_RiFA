# Controlador

## Histórico de Versões

| Data   | Versão | Descrição                       | Autor(es)      |
| ------ | ------ | ------------------------------- | -------------- |
| 04-Jan | 0.1    | Construção da Página            | Lucas Pimentel |
| 04-Jan | 0.2    | Adiciona introdução             | Lucas Pimentel |
| 04-Jan | 0.3    | Adiciona aplicação e introdução | Lucas Pimentel |
| 04-Jan | 0.4    | Arquivo revisado                | Eurico         |

## 1. Introdução

Um dos principais componentes do padrão GRASP é o controlador. O controlador tem o propósito de delegar eventos e regras de negócio para uma classe não-visual, orquestrando as operações do sistema, gerenciando a interação com os usuários e fazendo a ligação entre as diferentes partes do sistema. O controlador também pode ser responsável por tratar exceções e garantir a integridade dos dados.

O uso de um controlador pode ajudar a garantir que o sistema seja escalável e mantenível, pois permite que as responsabilidades sejam divididas de maneira clara entre as diferentes partes do sistema. Além disso, o uso de um controlador pode ajudar a garantir a coesão do sistema, quando não atribuido de muitas responsabilidades, pois ele centraliza a lógica de negócios em um único ponto.

No entanto, é importante notar que o uso de um controlador também pode levar a sistemas mais complexos, pois ele adiciona uma camada de abstração adicional. É importante avaliar cuidadosamente se o uso de um controlador é adequado para um determinado sistema e, se for o caso, garantir que ele seja implementado de maneira eficiente.

## 2. Aplicação no projeto

Sendo assim, por se tratar de um padrão de projeto amplamente utilizado, durante a elaboração do diagrama de pacotes do projeto já havíamos identificado a necessidade de implementar classes que fizessem o papel de controladores em nosso Front-end. Dessa forma, as controllers terão a função de coletar informações solicitadas pelos usuários nas classes de interface (pacote pages) e então delegar as solicitações feitas para as devidas classes do pacote service, como podemos ver pela imagem abaixo.

<center>

![Imagem](../../assets/Aplicacao_controler_e-rifas_2.png)

Figura 1 -> Fonte: Diagrama de pacotes do projeto

</center>

## 3. Conclusão

Em conclusão, o uso de classes controladoras pode ser extremamente útil em projetos de software complexos, pois permite atribuir responsabilidades de maneira clara e gerenciar a interação entre as diferentes partes do sistema, mantendo a coesão e o baixo acoplamento do código. No entanto, é importante tomar cuidado ao implementar, pois o uso de um controlador pode adicionar uma camada de abstração adicional e, se não for feito corretamente, pode levar a sistemas mais complexos e menos escaláveis em casos de controladores sobrecarregados. Com isso, cabe a equipe tomar decisões adequadas de quantas controladoras existirão no projeto e a responsabilidade de cada uma.

## Referências

- BEZERRA, Eduardo; SANTOS, Ismael. Modulo I Padrões GRASP. PUC-RIO - https://web.tecgraf.puc-rio.br/~ismael/Cursos/Cidade_FPSW/aulas/Modulo1_Intro_Grasp_GoF/Grasp/PadroesGRASP.pdf

- SERRANO, Milene. GRASPS - Material Complementar parte 1 - https://aprender3.unb.br/pluginfile.php/2277128/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20GRASP_A%20-%20Profa.%20Milene%20-%20Complementar.pdf

- CELESTINO, André. Design Patterns GRASP – Controller - https://www.andrecelestino.com/delphi-design-patterns-grasp-controller/
