### Diagrama de Casos de Uso

O **Diagrama de Casos de Uso** é um dos principais diagramas na UML (Unified Modeling Language) e é usado para capturar e descrever as funcionalidades de um sistema a partir da perspectiva do usuário. Ele foca nas interações entre os usuários (atores) e o sistema, mostrando o que o sistema deve fazer (casos de uso) e como os atores interagem com esses casos de uso.

#### Componentes Principais do Diagrama de Casos de Uso

1. **Atores (Actors)**:
   - Representam entidades externas ao sistema que interagem com ele. Eles podem ser pessoas, outros sistemas ou entidades externas.
   - São representados por figuras de bonecos ou ícones que se conectam aos casos de uso.

2. **Casos de Uso (Use Cases)**:
   - São as funcionalidades ou serviços que o sistema oferece aos atores. Cada caso de uso descreve um objetivo específico que um ator pode alcançar ao interagir com o sistema.
   - São representados por elipses com o nome do caso de uso.

3. **Relacionamentos**:
   - **Associação**: Linha sólida que conecta um ator a um caso de uso, mostrando que o ator participa do caso de uso.
   - **Inclusão (Include)**: Relacionamento entre casos de uso onde um caso de uso inclui a funcionalidade de outro caso de uso. Representado por uma linha com uma seta e o estereótipo `<<include>>`.
   - **Extensão (Extend)**: Relacionamento onde um caso de uso opcionalmente estende o comportamento de outro caso de uso. Representado por uma linha com uma seta e o estereótipo `<<extend>>`.
   - **Generalização**: Representa um relacionamento de herança entre atores ou casos de uso. Representado por uma linha com uma seta vazada.

#### Exemplo Gráfico de Diagrama de Casos de Uso

Vamos considerar um sistema simples de **Sistema de Biblioteca**. Os casos de uso típicos podem incluir:

1. **Cadastrar Livro**
2. **Empréstimo de Livro**
3. **Devolução de Livro**
4. **Consulta de Disponibilidade**
5. **Cadastro de Usuário**

#### Diagrama de Casos de Uso para o Sistema de Biblioteca

```plaintext
     +-------------------------+
     |                         |
     |      Sistema de         |
     |       Biblioteca        |
     |                         |
     +-------------------------+
            |        |
            |        |
     +------+----+   +------+
     |      Usuário      |   |   Bibliotecário    |
     +------------------+   +---------------------+
            |                       |
   +--------+--------+       +-------+-------+
   |                 |       |               |
   |     Cadastrar Livro    |       |  Empréstimo de Livro    |
   |                 |       |               |
   +--------+--------+       +-------+-------+
            |                       |
   +--------+--------+       +-------+-------+
   |                 |       |               |
   |   Devolução de Livro   |       |  Consulta de Disponibilidade  |
   |                 |       |               |
   +-----------------+       +---------------+
            |
   +--------+--------+
   |                 |
   |  Cadastro de Usuário |
   |                 |
   +-----------------+
```

#### Explicação do Exemplo

1. **Atores**:
   - **Usuário**: Pode interagir com o sistema para realizar ações como cadastrar livros, devolver livros, e consultar disponibilidade.
   - **Bibliotecário**: Realiza ações relacionadas ao empréstimo de livros e cadastro de novos livros.

2. **Casos de Uso**:
   - **Cadastrar Livro**: Permite ao bibliotecário adicionar novos livros ao sistema.
   - **Empréstimo de Livro**: Permite ao bibliotecário registrar o empréstimo de um livro para um usuário.
   - **Devolução de Livro**: Permite ao bibliotecário registrar a devolução de um livro.
   - **Consulta de Disponibilidade**: Permite ao usuário verificar se um livro está disponível para empréstimo.
   - **Cadastro de Usuário**: Permite ao bibliotecário registrar novos usuários no sistema.

3. **Relacionamentos**:
   - **Associações**: Mostram como os atores interagem com os casos de uso.
   - **Inclusão** e **Extensão**: Podem ser usados para modelar casos de uso que são frequentemente utilizados em outros casos de uso ou que adicionam funcionalidades adicionais.

#### Ferramentas para Criar Diagramas de Casos de Uso

Algumas ferramentas que suportam a criação de diagramas de casos de uso incluem:
- **Lucidchart**
- **Microsoft Visio**
- **Draw.io (diagrams.net)**
- **Enterprise Architect**
- **Visual Paradigm**

### Conclusão

O Diagrama de Casos de Uso é uma ferramenta essencial para modelar e entender as interações entre os usuários e o sistema, proporcionando uma visão clara das funcionalidades do sistema a partir da perspectiva dos usuários. Ele é fundamental para a análise de requisitos e para o design de sistemas centrados no usuário.

