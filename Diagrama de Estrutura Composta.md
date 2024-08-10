### Diagrama de Estrutura Composta (Composite Structure Diagram) na UML

O **Diagrama de Estrutura Composta** é um tipo de diagrama estrutural na UML (Unified Modeling Language) que detalha a estrutura interna de um classificador, mostrando como seus elementos internos colaboram para realizar um comportamento específico. Ele é usado para modelar a decomposição interna de um sistema, descrevendo a interação entre os seus componentes internos, como classes, interfaces, objetos, e seus relacionamentos.

#### Componentes Principais do Diagrama de Estrutura Composta

1. **Classificadores (Classifiers)**:
   - Representam entidades que possuem uma estrutura interna, como classes, componentes, ou nós. Esses classificadores são os "contêineres" dos elementos internos.

2. **Partes (Parts)**:
   - Representam os elementos internos de um classificador que compõem sua estrutura. Podem ser instâncias de classes, objetos, ou outros classificadores.
   - São representados por retângulos dentro do contêiner (classificador) que os possui.

3. **Portas (Ports)**:
   - As portas são pontos de interação com o exterior do classificador, usadas para enviar e receber mensagens. Elas definem como um classificador se comunica com o ambiente externo.
   - São representadas como pequenos quadrados ou círculos nas bordas do classificador.

4. **Conectores (Connectors)**:
   - Os conectores representam as linhas de comunicação entre as partes internas de um classificador. Eles mostram como as partes se comunicam para realizar o comportamento desejado.
   - São representados como linhas conectando as partes ou portas.

5. **Interfaces**:
   - Interfaces são tipos de portas que especificam as operações e serviços que as partes podem realizar ou consumir.

#### Quando Usar um Diagrama de Estrutura Composta?

- **Modelagem de Arquitetura Interna**: Para detalhar a estrutura interna de um sistema ou subsistema.
- **Especificação de Colaborações**: Para mostrar como diferentes elementos dentro de um classificador colaboram entre si.
- **Detalhamento de Componentes Complexos**: Quando um componente tem uma estrutura interna complexa que precisa ser descrita em detalhes.

### Exemplo Gráfico de Diagrama de Estrutura Composta

Vamos considerar um exemplo simples de um sistema de controle de tráfego aéreo, onde o sistema (classificador) é responsável por gerenciar as aeronaves no espaço aéreo.

#### Diagrama de Estrutura Composta:

```plaintext
+-----------------------------------+
| Sistema de Controle de Tráfego Aéreo |
|                                    |
| +-------------------------------+ |
| |         Radar (Parte)          | |
| +-------------------------------+ |
|          |                        |
| +-------------------------------+ |
| |      Comunicador (Parte)       | |
| +-------------------------------+ |
|          |                        |
| +-------------------------------+ |
| |       Computador (Parte)       | |
| +-------------------------------+ |
|                                    |
+-----------------------------------+
```

### Explicando o Exemplo

- **Classificador (Sistema de Controle de Tráfego Aéreo)**:
  - Representa o sistema geral responsável por gerenciar o tráfego aéreo. Ele é o contêiner das partes internas, como o radar, comunicador, e computador.

- **Partes**:
  - **Radar**: Uma parte do sistema que detecta aeronaves no espaço aéreo.
  - **Comunicador**: Uma parte responsável por se comunicar com as aeronaves e outras instalações.
  - **Computador**: Processa os dados recebidos e executa as operações de controle.

- **Conectores**:
  - As linhas entre as partes representam como esses componentes interagem entre si. Por exemplo, o Radar pode enviar dados de localização para o Computador, que então os processa e envia comandos para o Comunicador.

### Comparação com Outros Diagramas

- **Diagrama de Classes**: Foca nas relações estáticas entre classes, como herança e associações.
- **Diagrama de Componentes**: Foca na organização dos componentes de software em um sistema.
- **Diagrama de Estrutura Composta**: Foca na estrutura interna de um classificador e como seus componentes colaboram.

### Ferramentas para Criar Diagramas de Estrutura Composta

Algumas ferramentas populares incluem:
- **Enterprise Architect**
- **Lucidchart**
- **Visual Paradigm**
- **Microsoft Visio**
- **Draw.io**

Estas ferramentas permitem criar diagramas de estrutura composta de maneira intuitiva, ajudando a visualizar a arquitetura interna de sistemas complexos.

### Conclusão

O Diagrama de Estrutura Composta é uma ferramenta poderosa para modelar a estrutura interna de sistemas complexos, oferecendo uma visão detalhada de como os elementos internos de um classificador colaboram. Ele é essencial para a documentação e entendimento de sistemas onde a interação interna entre componentes é crucial para o comportamento do sistema como um todo.

