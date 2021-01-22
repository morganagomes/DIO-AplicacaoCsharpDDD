## Desenvolvendo aplicação com C# usando DDD :desktop_computer:

Projeto realizado durante a aula **Desenvolvendo aplicação com C# usando DDD** pelo instrutor Alexandre Daccas. O presente projeto faz parte das atividades requisitadas no **Bootcamp Decola Dev 2021**, uma parceria da Digital Innovation One e da Avanade. :orange:

-----

:writing_hand: <u>Pontos importantes</u>¹:

1. O que é DDD?

- DDD (_Domain Driven Design_) é uma abordagem de design de software que reúne um conjunto de conceitos, técnicas e princípios de softwares baseados em um modelo de domínio (todo e qualquer conhecimento da área).
- A origem do DDD vem do título do livro escrito por Eric Evans que catalogou padrões baseados nas suas experiências com desenvolvimento de software e no uso de técnicas de orientação a objetos.



2. Principais conceitos do DDD:

- **Alinhamento do código com o negócio**: contato dos desenvolvedores com os especialistas do domínio.
- **Favorecer a reutilização**: aproveitar um mesmo conceito de domínio e um mesmo código de vários lugares.
- **Mínimo de acoplamento**: modelo organizado de forma que não haja muita dependência entre módulos ou classes de objetos de conceitos distintos.
- **Independência da tecnologia**: não há um foco na tecnologia, mas sim nas regras de negócio e em como elas devem estar refletidas no código e no modelo de domínio.



3. Criação de um Modelo de Domínio (MDD)

- O modelo abstrato deve ser uma representação perfeita do domínio.
- O desenho do modelo é criado em conjunto entre especialistas de negócio e domínios, analistas, arquitetos e desenvolvedores.
- Utiliza linguagem ubíqua.
- O processo de maturação de um sistema desenvolvido usando em MDD é contínuo.



4. Blocos de construção do MDD

- **Interface do usuário**: responsável pela exibição de informações do sistema ao usuário.
- **Aplicação**: responsável por conectar a interface de usuário às camadas inferiores.
- **Domínio**: representa os conceitos, regras e lógicas do negócio. Todo foco do DDD está nessa camada.
- **Infra-estrutura**: fornece recursos técnicos que darão suporte às camadas superiores.



5. Arquitetura padrão do MDD

![img](http://www.agileandart.com/wp-content/uploads/2010/07/Screen-shot-2010-07-16-at-09.50.18.png)



6. Regras para modelagem

- **Entidades**: classes de objetos que necessitam de uma identidade.
- **Objetos de Valores**: objetos que só carregam valores, mas que não possuem distinção de identidade. Por exemplo: strings, números ou cores. As instâncias de Objetos de Valores são imutáveis, isto é, uma vez criados, seus atributos internos não poderão mais ser modificados.

- **Agregados**: compostos de Entidades ou Objetos de Valores que são encapsulados numa única classe. Servem para manter a integridade do modelo.
- **Fábricas**: classes responsáveis pelo processo de criação de Agregados ou dos Objetos de Valores.
- **Serviços**: classes que contém lógica de negócio, mas que não pertencem a nenhuma Entidade ou Objetos de Valores. 
- **Repositórios**: classes responsáveis por administrar o ciclo de vida dos outros objetos normalmente Entidades, Objetos de Valor e Agregados. Centralizam operações de criação, alteração e remoção de objetos.
- **Módulos**: agrupam classes por um determinado conceito do domínio



7. Exemplos de implementação

Aplicação com C# usando DDD elaborado por [Alex Alves](https://github.com/alexalvess/aurora-api-project.git) .



[^1]: Breve fichamento do que foi apresentado durante a aula.