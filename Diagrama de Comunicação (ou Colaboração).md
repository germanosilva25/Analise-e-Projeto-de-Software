O **Diagrama de Comunicação** (ou Diagrama de Colaboração) é um tipo de diagrama na UML (Unified Modeling Language) que mostra as interações entre objetos ou componentes em um sistema. Ele ilustra como os objetos colaboram para realizar uma tarefa específica, destacando as mensagens trocadas e a relação entre os objetos.

### Componentes Principais do Diagrama de Comunicação

1. **Objetos**:
   - Representados por retângulos com o nome do objeto e, ocasionalmente, sua classe. Os objetos são dispostos ao redor do diagrama, conectados por linhas para representar interações.

2. **Mensagens**:
   - Setas que conectam os objetos, representando a comunicação entre eles. As mensagens são numeradas para indicar a ordem em que são enviadas.

3. **Links**:
   - Linhas conectando os objetos, representando a associação ou comunicação entre eles.

4. **Notas e Comentários**:
   - Informações adicionais podem ser incluídas no diagrama para fornecer contexto ou esclarecer detalhes.

### Exemplo Gráfico de Diagrama de Comunicação

Vamos considerar um exemplo de um sistema de **Reserva de Hotel**, onde um cliente faz uma reserva. O diagrama de comunicação para este processo pode ser descrito da seguinte forma:

#### Descrição do Processo

1. O **Cliente** solicita uma reserva.
2. O **Sistema de Reserva** verifica a disponibilidade.
3. O **Sistema de Reserva** confirma a reserva.
4. O **Sistema de Reserva** notifica o **Cliente**.

#### Diagrama de Comunicação

```plaintext
+---------+                +-----------------+              +-------------+
| Cliente |                | Sistema de      |              | Banco de    |
|         |                | Reserva          |              | Dados       |
+---------+                +-----------------+              +-------------+
    |                               |                              |
    |--- Solicitar Reserva --------->|                              |
    |                               |--- Verificar Disponibilidade ->|
    |                               |                              |--- Consultar Disponibilidade ->|
    |                               |                              |<-- Disponibilidade Confirmada ---|
    |                               |<-- Reserva Confirmada --------|
    |<-- Notificar Reserva ----------|
    |                               |                              |
```

#### Explicação do Exemplo

1. **Cliente**:
   - **Solicitar Reserva**: O cliente solicita uma reserva no sistema.
2. **Sistema de Reserva**:
   - **Verificar Disponibilidade**: O sistema de reserva verifica a disponibilidade com o banco de dados.
   - **Confirmar Reserva**: Após confirmar a disponibilidade, o sistema confirma a reserva.
   - **Notificar Reserva**: O sistema notifica o cliente sobre a confirmação da reserva.
3. **Banco de Dados**:
   - **Consultar Disponibilidade**: O banco de dados é consultado para verificar a disponibilidade.

### Como Criar um Diagrama de Comunicação

1. **Identificar os Objetos**: Determine os objetos ou componentes que participam da interação.
2. **Desenhar os Objetos**: Coloque os objetos no diagrama e desenhe os links entre eles.
3. **Adicionar Mensagens**: Conecte os objetos com setas que representam as mensagens trocadas, numerando-as para mostrar a ordem.
4. **Incluir Notas e Comentários**: Adicione qualquer informação adicional para esclarecer o diagrama.

### Ferramentas para Criar Diagramas de Comunicação

Algumas ferramentas que permitem criar diagramas de comunicação incluem:

- **Lucidchart**
- **Microsoft Visio**
- **Draw.io (diagrams.net)**
- **Enterprise Architect**
- **Visual Paradigm**

### Conclusão

O Diagrama de Comunicação é útil para visualizar como os objetos em um sistema colaboram para executar um processo específico. Ele destaca a estrutura de comunicação e as interações entre os objetos, ajudando a entender o fluxo de mensagens e as relações entre os componentes do sistema.

