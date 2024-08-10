O **Diagrama de Estados** (ou Diagrama de Máquinas de Estado) na UML (Unified Modeling Language) é um tipo de diagrama que descreve o comportamento de um sistema ou de um componente específico, mostrando como ele muda de estado em resposta a eventos. Ele é particularmente útil para modelar o comportamento de objetos que possuem estados distintos e transições entre esses estados.

### Componentes Principais do Diagrama de Estados

1. **Estados**:
   - Representam as diferentes condições ou situações que um objeto pode estar. São geralmente representados por retângulos com bordas arredondadas.
   - **Estado Inicial**: Representado por um círculo preenchido, indicando o estado em que o objeto começa.
   - **Estado Final**: Representado por um círculo com um ponto no meio, indicando o estado final do ciclo de vida do objeto.

2. **Transições**:
   - Representam a mudança de um estado para outro em resposta a um evento. São desenhadas como setas entre os estados.
   - **Eventos**: São as condições que causam a transição entre estados.
   - **Ações**: São operações realizadas durante uma transição ou quando um estado é ativado.

3. **Transições Internas**:
   - Transições que ocorrem dentro de um estado sem mudar para um estado diferente. São desenhadas como setas internas dentro do estado.

4. **Decisões**:
   - Pontos onde o fluxo pode se dividir em diferentes caminhos com base em uma condição. Representados por losangos.

5. **Habilidades**:
   - Representam ações que podem ser realizadas pelo sistema ou objeto enquanto está em um determinado estado.

### Exemplo Gráfico de Diagrama de Estados

Vamos considerar um exemplo de um **Pedido de Compra** em um sistema de e-commerce. O diagrama de estados pode ilustrar os diferentes estados que um pedido pode atravessar e as transições entre esses estados.

#### Descrição dos Estados

1. **Pedido Criado**: Estado inicial quando o pedido é criado.
2. **Em Processamento**: Quando o pedido está sendo processado.
3. **Enviado**: Quando o pedido foi enviado para o cliente.
4. **Entregue**: Quando o pedido é entregue ao cliente.
5. **Cancelado**: Se o pedido é cancelado em qualquer momento.

#### Diagrama de Estados

```plaintext
  +----------------+           +-----------------+
  | Pedido Criado  |           |   Em Processamento  |
  +----------------+           +-----------------+
         |                               |
         v                               v
  +----------------+           +-----------------+
  |     Enviado    |<----------|   Pedido Cancelado   |
  +----------------+           +-----------------+
         |
         v
  +----------------+
  |   Entregue     |
  +----------------+
```

#### Explicação do Exemplo

1. **Pedido Criado**:
   - **Transição**: Quando o pedido é criado, ele entra no estado de "Pedido Criado".
2. **Em Processamento**:
   - **Transição**: O pedido move-se para "Em Processamento" quando começa a ser processado.
   - **Evento**: Recebimento do pedido.
3. **Enviado**:
   - **Transição**: O pedido é enviado para o cliente.
   - **Evento**: Pedido enviado.
4. **Entregue**:
   - **Transição**: O pedido chega ao cliente e é marcado como "Entregue".
   - **Evento**: Pedido entregue.
5. **Cancelado**:
   - **Transição**: O pedido pode ser cancelado a qualquer momento, movendo-o para o estado "Cancelado".
   - **Evento**: Cancelamento do pedido.

### Como Criar um Diagrama de Estados

1. **Identificar Estados**: Determine todos os estados possíveis de um objeto ou sistema.
2. **Desenhar Estados**: Coloque os estados no diagrama e desenhe o estado inicial e final.
3. **Adicionar Transições**: Conecte os estados com setas que representam transições, e indique os eventos que causam essas transições.
4. **Incluir Decisões e Ações**: Adicione decisões e ações conforme necessário para representar a lógica de transição.

### Ferramentas para Criar Diagramas de Estados

Algumas ferramentas que permitem criar diagramas de estados incluem:

- **Lucidchart**
- **Microsoft Visio**
- **Draw.io (diagrams.net)**
- **Enterprise Architect**
- **Visual Paradigm**

### Conclusão

O Diagrama de Estados é essencial para modelar o comportamento de sistemas e objetos com base em seus estados e transições. Ele fornece uma visão clara de como um sistema reage a eventos e como seus estados mudam ao longo do tempo. Esse tipo de diagrama é valioso para entender e projetar a lógica de estados e comportamentos em sistemas complexos.