<div id="top"></div>

<br/>
<div align="center">
    <img src="./readme-img/3d-modeling.png" alt="Logo" width="100" height="100" />
    <h1 align="center">Fundamentos de Arquitetura de Software</h1>
    <p align="center">OOP - SOLID - Dependency Injection - Clean Code - Design Patterns</p>
</div>

<br/>

<div align="center">
    <a href="https://github.com/YuriSiman/software-architecture-fundamentals/blob/master/LICENSE" target="_blank">
      <img alt="LICENSE" src="https://img.shields.io/badge/license-mit-%23A6CE39?style=for-the-badge&logo=github" />
    </a>
    <a href="https://github.com/YuriSiman" target="_blank">
      <img alt="GitHub" src="https://img.shields.io/badge/github-perfil-%237159c1?style=for-the-badge&logo=github" />
    </a>
    <a href="https://yurisiman.com.br" target="_blank">
      <img alt="Site" src="https://img.shields.io/badge/site-yurisiman-E0A80D?style=for-the-badge&logo=Purism" />
    </a>
    <a href="https://www.linkedin.com/in/yurisiman/" target="_blank">
      <img alt="Linkedin" src="https://img.shields.io/badge/linkedin-social-0A66C2?style=for-the-badge&logo=LinkedIn" />
    </a>
    <a href="mailto:contato@yurisiman.com.br" target="_blank">
      <img alt="Gmail" src="https://img.shields.io/badge/email-contato-EA4335?style=for-the-badge&logo=Gmail" />
    </a>
</div>

<br/>

## :clipboard: Sobre o Projeto

Este projeto tem como objetivo implementar os principais conceitos a respeito dos fundamentos de software para que possa servir de estudo e consulta sobre o tema. Trata-se de uma aplicação que tem como único propósito a descrição e exemplificação de fundamentos de arquitetura de software. Desenvolvido em C# abordando conceitos de OOP - SOLID - Dependency Injection - Clean Code - Design Patterns.

---

## :pencil: Pré-requisitos

1. Construído com .NET 5.0 e codificado em C#, se você não possui o dotnet instalado, acesse [aqui](https://dotnet.microsoft.com/) e instale a versão mais recente.
2. Clone este repositório em sua máquina local

   ```sh
   git clone https://github.com/YuriSiman/software-architecture-fundamentals.git
   ```

---

## :dart: Tópicos

<details>
  <summary>Fundamentos</summary>
  <ul>
    <li><a href="#arquitetura">O que é Arquitetura?</a></li>
    <li><a href="#oop">OOP</a></li>
    <li><a href="#solid">SOLID</a></li>
    <li><a href="#clean-code">Clean Code</a></li>
    <li><a href="#design-patterns">Design Patterns</a></li>
    <li><a href="#estilos-e-padroes-arquiteturais">Estilos e Padrões Arquiteturais</a></li>
    <li><a href="#devops">DevOps</a></li>
  </ul>
</details>

---

## :rocket: Vamos Começar

### Fundamentos

<div id="arquitetura"></div>

### O que é Arquitetura?    

"Arquitetura é a organização fundamental de um sistema incorporada em seus componentes, relacionamentos com o ambiente e os princípios que conduzem seu design e evolução." [ISO/IEC/IEEE 42010-2011](https://www.iso.org/standard/50508.html)  

Como construir software:  

<div align="center">
    <img src="./readme-img/arquitetura-software.png" width="900" height="500" />
</div>

#### TOGAF

The Open Group Architecture Framework (TOGAF) é um framework de arquitetura corporativa que provê uma abordagem global ao design, planejamento, implementação e governança de uma arquitetura corporativa.  

[OpenGroup](https://www.opengroup.org/togaf)

#### ISO/IEC/IEEE 42010-2011  

Engenharia de sistemas e software ISO / IEC / IEEE 42010 - A descrição da arquitetura é um padrão internacional para descrições de arquitetura de sistemas e software.

[ISO/IEC/IEEE 42010-2011](https://www.iso.org/standard/50508.html)

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="oop"></div>

### OOP    

É essencial possuir um claro conhecimento dos princípios da orientação a objetos para poder aplicar as melhores práticas de design de código, padrões e abordagens de arquitetura. Na orientação a objetos devemos sempre buscar o baixo acoplamento e a alta coesão entre os objetos, ou seja, evitar uma dependência direta entre um objeto e outro, tendo os objetos executando uma única responsabilidade livres de uma dependência direta com outros.

Pilares da Programação Orientada a Objetos

<div align="center">
    <img src="./readme-img/pilares-oop.png"/>
</div>

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="solid"></div>

### SOLID    

<div align="center">
    <img src="./readme-img/solid.png" />
</div>
<br/>

SOLID é um acrônimo dos cinco primeiros princípios da programação orientada a objetos e design de código identificados por Robert C. Martin (Uncle Bob) por volta do ano 2000. Os princípios SOLID devem ser aplicados para se obter os benefícios da orientação a objetos, como:

- Seja fácil de se manter, adaptar e se ajustar às alterações de escopo
- Seja testável e de fácil entendimento
- Seja extensível para alterações com o menor esforço necessário
- Que forneça o máximo de reaproveitamento
- Que permaneça o máximo de tempo possível em utilização

Problemas comuns que conseguimos evitar quando utilizamos os princípios SOLID:

- Dificuldade na testabilidade / criação de testes de unidade
- Código macarrônico, sem estrutura ou padrão
- Dificuldades de isolar funcionalidades
- Duplicação de código, uma alteração precisa ser feita em N pontos
- Fragilidade, o código quebra facilmente em vários pontos após alguma mudança

#### SRP - Single Responsability Principal

Uma classe deve ter um,e apenas um, motivo para ser modificada.

#### OCP - Open Closed Principle

Entidades de software (classes, módulos, funções, etc...) devem estar abertas para extensão, mas fechadas para modificação.

#### LSP - Liskov Substitution Principle

O principal objetivo do LSP é questionar se o desenvolvedor está realizando uma herança dentro dos padrões de design e abstração ou está apenas seguindo a linha do "é um...". Subclasses devem ser substituíveis por suas Superclasses. Este princípio reswolve o problema de heranças que não deveriam ser implementadas.

Se q(x) é uma propriedade demonstrável dos objetos x de tipo T. Então q(y) deve ser verdadeiro para objetos y de tipo S onde S é um subtipo de T.

#### ISP - Interface Segregation Principle

Clientes não devem ser forçados a depender de métodos que não usam. Muitas interfaces específicas são melhores do que uma interface única. Delegar contratos (interfaces) é uma forma de garantir design e abstração do código.

#### DIP - Dependency Inversion Principle

Módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações. Abstrações não devem depender de detalhes. Detalhes devem depender de abstrações.

Dependa de uma abstração e não de uma implementação.

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="clean-code"></div>

### Clean Code      

#### O que é um código limpo?

- Simples
- Direto
- Eficiente
- Sem duplicidade
- Elegante
- Feito com cuidado
- Fácil de ler

"Qualquer tolo consegue escrever código que um computador entenda. Bons programadores escrevem código que humanos possam entender". Martin Fowler

#### Quanto custa um código ruim?

- Alta rotatividade
- Demora na entrega de novas funcionalidades
- Dificuldade na manutenção
- Alta incidência de bugs
- Perda de confiança do cliente
- Desmotivação profissional
- Mais tempo depurando o código do que escrevendo

#### Como medir um bom código?

- Quantidade de linhas de código (Devemos buscar reduzir ao máximo o tamanho do código, dependendo do projeto)
- Número de métodos (Devemos buscar utilizar a maior quantidade de métodos para um desacoplamento maior)
- Número de classes (Devemos buscar utilizar a maior quantidade de métodos para um desacoplamento maior)
- Linhas de código por método (Devemos buscar reduzir a quantidade de linhas dentro do método)
- Complexidade ciclomática (Evitar uma grande quantidade de caminhos de execução independentes, ou seja, evitar if's encadeados)
- Número de estruturas de decisão (Evitar um exagero de estruturas de decisão)
- Escolher os nomes que revelem intenção (Revelando o motivo dele existir, o que faz e como é usado. Utilizar nomes fáceis de se encontrar, evitando siglas ou acrônimos. Não economizar palavras para dar nome a alguma coisa)

#### Boas práticas

- Nome de classes devem ser substantivos e não devem conter verbos. Ex: ClienteRepository
- Nomes de métodos devem conter verbos de preferência no infinitivo. Ex: AdicionarCliente
- Não ser genérico. Ex: ProcessarFolhaPagamento / CalcularImpostoRenda
- Menos é mais! "A primeira regra dos métodos é que eles devem ser pequenos. A segunda regra é que eles devem ser menores ainda". Uncle Bob

  - Métodos <= 20 linhas
  - Linha <= 100 caracteres
  - Classe <= 500 linhas
- Extraia trechos de métodos privados
- Métodos devem fazer apenas uma coisa, fazê-la certa e somente fazê-la
- Evite muitos parâmetros em métodos
- Não deixe o método mentir dizendo que faz uma coisa mas na verdade faz outras "escondidas"
- Se o método tiver mais de uma responsabilidade, extraia em dois ou mais
- Leia seu método de cima para baixo como uma narrativa, ele deve fazer sentido
- Aplique uma boa indentação

#### Comentários

- Comentários não vão ajudar um código ruim ser melhor interpretado
- Um código que requer comentário precisa ser reescrito
- Não deixe trechos de código comentado

#### Quando comentar?

- Alertar consequências que podem vir a causar
- Licença, direitos autorais, etc...
- Necessidade de explicar uma regra de negócio interna
- Decisões de design de código
- Utilizar comentários quando os mesmos geram uma documentação do código (Ainda assim, não é tão recomendado)

#### Tratamento de erros

- Tratar e prever possíveis exceções é de responsabilidade do desenvolvedor
- Retorne exceptions e não códigos de erro
- Informe o máximo que puder em sua exception
- Se necessário crie exceptions personalizadas para um problema específico
- Não retorne null

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="design-patterns"></div>

### Design Patterns      

Design Patterns são padrões de código para solução de problemas conhecidos. O objetivo não é reinventar a roda, mas sim aplicar uma solução com um bom design de código. O conceito de padrões foi introduzido por 4 desenvolvedores intitulados Gang of Four (GoF) e hoje conta com 23 padrões fundamentais. Atualmente existem mais de 80 padrões conhecidos que são em geral variações dos 23 patterns do GoF.

<div align="center">
    <img src="./readme-img/patterns.png" />
</div>
<br/>

Os padrões do GoF estão divididos em 3 famílias:

Família | Descrição
--------|----------
Creational Patterns (Criacional) | Fornecem meios de criação de um objeto e de como ele será instanciado
Structural Patterns (Estrutural) | Tratam da composição de objetos por heranças e interfaces para diferentes funcionalidades
Behavioral Patterns (Comportamental) | Tratam das interações e comunicação entre os objetos além da divisão de responsabilidades

[.NET Design Patterns](https://dofactory.com/net/design-patterns)

#### Creational Patterns

- Abstract Factory

Cria uma instância de diversas famílias de classes. Criar fábrica abstrata de fábricas.

<div align="center">
    <img src="./readme-img/abstract-factory.png" />
</div>
<br/>

- Factory Method

Cria uma instância de diversas derivações de classes.

<div align="center">
    <img src="./readme-img/factory-method.png" />
</div>
<br/>

- Singleton

Cria uma única instância que será utilizada por os recursos

<div align="center">
    <img src="./readme-img/singleton.png" />
</div>
<br/>

<p align="right"><a href="#top">Início ↑</a></p>

#### Structural Patterns

- Adapter

Compatibiliza objetos de interfaces diferentes

<div align="center">
    <img src="./readme-img/adapter.png" />
</div>
<br/>

- Facade

Uma única classe que representa um subsistema

<div align="center">
    <img src="./readme-img/facade.png" />
</div>
<br/>

- Composite

Compartilha um objeto em estruturas de árvores que representam hierarquias

<div align="center">
    <img src="./readme-img/composite.png" />
</div>
<br/>

<p align="right"><a href="#top">Início ↑</a></p>

#### Behavioral Patterns

- Command

Encapsula um command request em um objeto

<div align="center">
    <img src="./readme-img/command.png" />
</div>
<br/>

- Strategy

Encapsula um algoritimo dentro de uma classe

<div align="center">
    <img src="./readme-img/strategy.png" />
</div>
<br/>

- Observer

Uma forma de notificar mudanças a uma série de classes

<div align="center">
    <img src="./readme-img/observer.png" />
</div>
<br/>

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="estilos-e-padroes-arquiteturais"></div>

### Estilos e Padrões Arquiteturais      

Um estilo arquitetura é uma abordagem de como projetar e entregar uma aplicação. Trata-se de como organizar os componentes responsáveis de uma arquitetura, como eles irão interagir entre si e quais aspectos tecnológicos irão atender.

- Arquitetura Monolítica
- Arquitetura em Camadas
- Arquitetura REST
- Arquitetura de Microservices
- Arquitetura de Plugin
- Arquitetura Client-Server
- Arquitetura Pines and Filters

Os Padrões Arquiteturais são semelhantes aos "Design Patterns", mas possuem um escopo diferente. Padrões Arquiteturais são estratégias de alto nível que dizem respeito a componentes de grande escala, as propriedades e mecanismos globais de um sistema. Um projeto de arquitetura pode conter diversos estilos arquiteturais, e cada estilo arquitetural pode utilizar diversos padrões arquiteturais. Um padrão arquitetural pode ser um subconjunto de um estilo arquitetural visando um escopo específico. O padrão arquitetural é uma solução geral e reutilizável para um problema em um contexto particular. É uma solução recorrente para um problema recorrente.

- Tier Architecture (Arquitetura 3 camadas)

Cássica maneira de distribuir responsabilidades (apresentação, aplicação/negócios e acesso a dados). Pode ser aplicada em diversos cenários, porém geralmente é mais encontrada em aplicações com foco comercial.

- Onion Architecture (Arquitetura Cebola - Clean Architecture)

Padrão Arquitetural que, para chegar na camada mais interna, é necessário passar pelas camadas externas.

- Arquitetura Hexagonal (Ports & Adapters)

Tem como objetivo implementar a Onion Architecture, DDD, Clean, CQRS, mensageria... tudo junto na mesma aplicação. Permite que seja possível fazer qualquer coisa na arquitetura.

- CQRS - Command Query Responsibility Segregation

Um padrão arquitetural onde o foco principal é separar os meios de leitura e escrita de dados. Alterações de dados são realizados via Commands e leitura de dados são realizados via Queries. O objetivo do CQRS é prover expressividade para aplicação, pois todos os Commands representam uma intenção de negócio. CQRS promove a consistência eventual, que é quando possuímos um banco de leitura e outro de escrita com os mesmos dados, porém os dados não são consistidos exatamente no mesmo momento. Muito aplicado em arquiteturas hexagonais, microservices ou em aplicações que possuem uma alta demanda de consumo de dados.

Commands: Representam uma intenção de mudanças no estados de uma entidade. São expressivos e representam uma única intenção de negócio. Queries: É a forma de obter dados de um banco ou origem de dados para atender as necessidades da aplicação.

- Event Sourcing

É um Padrão Arquitetural - "Nós podemos buscar o estado de uma aplicação para encontrar o estado atual do mundo, e isso responde muitas perguntas. Entretanto há momentos que nós não só querermos ver onde nós estamos, mas também queremos saber como chegamos lá." - Martin Fowler.

"Event Sourcing assegura que todas as mudanças feitas no estados de uma aplicação são armazenadas como uma sequência de eventos. Não só podemos buscar esses eventos, mas também podemos usar este log de eventos para reconstruir estados passados e ajustar automaticamente o estado atual com mudanças retroativas." - Martin Flowler

A ideia central é persistir todos estados anteriores de uma entidade de negócio desde o momento de sua ciraçãop. Com estes dados é possível realizar o "replay" dos fatos passados para entender o comportamento do usuário, trabalhar com Big Data, Machine Learning, realizar testes de integração com cenários reais ou simplesmente recriar as entidades se necessário.

- DDD (Domain-Driven Design)

Indicado para aplicações complexas, com muitas entidades e regras de negócio. Um "guia" de como entender o negócio, organizá-lo em um conjunto de princípios, criar uma modelagem com base no negócio e implementar utilizando diversas boas práticas.

Processos de "implementação" do DDD:

- Entender o negócio
- Extrair a Linguagem Ubíqua (Vocabulário de todos os termos específicos do domínio)
- Modelagem Estratégica (Segregar seu domínio em partes menores e responsáveis com Mapa de Contextos - Context Map - que pode ser representado através de imagens e uma simples documentação do tipo de relacionamento entre os contextos)
- Definir a Arquitetura
- Modelagem Tática
  - Aggregate Object: Uma entidade que é a raiz agregadora de um processo do domínio que envolve mais de uma entidade.
  - Domain Model: Uma entidade do domínio, possui estados e comportamentos. lógica de negócios, getters e setters AdHoc, etc...
  - Value Object: Um objeto que agrega valor às entidades, não possui identidade e é imutável.
  - Factory: Classe responsável por construir adequadamente um objeto / entidade.
  - Domain Service: Serviço do domínio que atende partes do negócio que não se encaixam em entidades específicasq, trabalha com diversas entidades, realiza persistência através de repositórios e etc...
  - Application Service: Serviço de aplicação que orquestra ações disparadas pela camada de apresentação e fornece DTO's para comunicação entre as demais camadas e para o consumo da camada de apresentação.
  - Repository: Uma classe que realiza a persistência das entidades se comunicando diretamente com o meio de acesso aos dados, é utilizado apenas um repositório por agregação.
  - External Service: Serviço externo que realiza a consulta/persistência de informações por meios diversos.

- Arquiteturas Evolutivas

"Um arquiteto permite que decisões importantes sejam adiadas e um bom arquiteto maximiza o número de decisões não tomadas." - Uncle Bob

"Uma arquitetura evolutiva suporta mudanças contínuas e incrementais como um primeiro princípio por meio de vários aspectos." - Rebecca Parsons

"Mudanças são inevitáveis. A evolução, no entando, é opcional." - Tony Robbins

<p align="right"><a href="#top">Início ↑</a></p>

---

<div id="devops"></div>

### DevOps      

O termo DevOps deriva da junção das palavras desenvolvimento (developer) e operações (operations), sendo uma prática de engenharia de software que possui o intuito de unificar o desenvolvimento de software (Dev) e a operação de software (Ops). A característica principal do movimento DevOps é defender fortemente a automação e monitoramento em todas as fases da construção do software, da integração, teste, liberação para implantação e gerenciamento de infraestrutura. DevOps pretende fornecer, em ciclos de desenvolvimentos menores, frequência de implantação aumentada, liberações mais seguras, em alinhamento próximo com os ojetivos de negócio.

<p align="right"><a href="#top">Início ↑</a></p>

---

## :vertical_traffic_light: Status do Projeto

:heavy_check_mark: Concluído

---

## :thinking: Contribuindo

> Passo a passo de como contribuir...

### Passo 1

* :fork_and_knife: Fork este repositório!

### Passo 2

* :dancers: Clone este repositório para sua máquina local usando `git clone https://github.com/YuriSiman/software-architecture-fundamentals.git`

### Passo 3

* :trident: Crie sua feature branch usando `git checkout -b minha-feature`

### Passo 4

* :white_check_mark: Commit suas mudanças usando `git commit -m "feat: Minha nova feature"`

### Passo 5

* :pushpin: Dê um push usando `git push -u origin minha-feature`

### Passo 6

* :arrows_clockwise: Crie um novo pull request

Depois que seu pull request for mesclado, você pode excluir sua feature branch  

> Caso tenha dúvidas, confira este guia de como [contribuir no GitHub](https://github.com/firstcontributions/first-contributions)  

---

## :speech_balloon: Suporte

> Entre em contato comigo...  

* Me chame pelo [Linkedin](https://www.linkedin.com/in/yurisiman/)  
* Me mande um e-mail [contato@yurisiman.com.br](mailto:contato@yurisiman.com.br)  

---

## :pencil: Licença

<a href="https://github.com/YuriSiman/software-architecture-fundamentals/blob/master/LICENSE" target="_blank">
  <img alt="LICENSE" src="https://img.shields.io/badge/license-mit-%23A6CE39?style=for-the-badge&logo=github" />
</a>

##

Code your life :octocat:

<p align="right"><a href="#top">Início ↑</a></p>
