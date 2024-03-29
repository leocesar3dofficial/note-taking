# BPMN (Business Process Model and Notation)

## Características

- Representação gráfica dos processos de um sistema

## Boas práticas

- Definir inícios e fins claros.
- Manter claro os cenários primários e alternativos.
- Definir marcos (milestones)
- Usar os padrões BPMN (standards).
- Simplificar diagramas.

## Elementos

### Eventos

- Início (Start)
- Intermediário (Intermediate)
- Fim (End)

### Atividades

- Tarefa
- Sub processo (Quadrado simples com +)
- Transação
- Chamar atividade

### Conexões

- Fluxo de sequência (\_\_\_➤)
- Fluxo de mensagem (◇.....➢)
- Associação (.....)

### Gateways

- Exclusive (Exclusivo, X)
  - Representa uma decisão onde apenas uma das saídas é escolhida, com base em uma condição
  - Apenas uma das sequências de saída será seguida, dependendo da avaliação da condição associada
- Inclusive (Inclusivo, O)
  - Permite que múltiplas sequências de saída sejam seguidas, com base em condições avaliadas
  - Mais de uma sequência pode ser escolhida, dependendo das condições definidas
- Parallel (Paralelo, +)
  - Divide o fluxo de execução em múltiplos caminhos paralelos
  - Todas as sequências de saída são seguidas simultaneamente, sem depender de condições
- Complex (Complexo, \*)
  - É um gateway mais flexível que permite modelar condições complexas para a decisão do fluxo
  - Ele pode ter várias entradas e saídas, permitindo lógicas mais elaboradas
- Event-Based (Baseado em Evento, Pentágono)
  - É usado para modelar fluxos condicionais com base em eventos
  - As sequências de saída são ativadas por eventos específicos que ocorrem durante a execução do processo
  - Círculo duplo com pentágono: apenas Event-Based
  - Círculo simples com pentágono: Event-Based exclusivo
  - Círculo simples com +: Event-Based paralelo

## ARIS-EPC (Event-driven Process Chain)

- Notação de modelagem de processos de negócios.
- Ênfase em eventos e em transições de estados.