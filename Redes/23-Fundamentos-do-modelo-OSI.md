# Aula — Fundamentos do Modelo OSI

## Os três pilares da comunicação em redes

A comunicação entre computadores é organizada por camadas. Para entender como elas funcionam, precisamos conhecer três conceitos fundamentais: **interfaces, protocolos e serviços**.

### 1. Interfaces

São os pontos de comunicação entre camadas vizinhas de um mesmo sistema.

A interface define como uma camada acessa os recursos e funcionalidades oferecidos pela camada imediatamente inferior.

**Exemplo:** uma camada utiliza os serviços da camada abaixo para realizar suas funções, sem precisar conhecer todos os detalhes internos dela.

### 2. Protocolos

São conjuntos de regras que determinam como entidades de uma mesma camada se comunicam em dispositivos diferentes.

Essas regras definem como as informações devem ser organizadas, transmitidas e interpretadas.

**Exemplo:** dois computadores precisam seguir regras compatíveis para conseguir trocar informações corretamente.

### 3. Serviços

Representam as funcionalidades que uma camada oferece à camada imediatamente superior.

Uma camada utiliza os serviços da camada inferior e, ao mesmo tempo, pode oferecer serviços à camada acima.

**Exemplo:** uma camada solicita à camada inferior que realize determinada tarefa, sem precisar conhecer como ela executa essa tarefa internamente.

## Diferença entre os três conceitos

| Conceito | Função |
|---|---|
| Interface | Define a comunicação entre camadas vizinhas. |
| Protocolo | Define as regras de comunicação entre entidades de mesma camada. |
| Serviço | Define o que uma camada oferece à camada superior. |

## Para memorizar

- **Interface:** como uma camada acessa a camada vizinha.
- **Protocolo:** regras de comunicação entre camadas equivalentes.
- **Serviço:** o que uma camada oferece à camada superior.

> **Atenção:** este resumo foi elaborado com base na descrição da aula enviada. Ele organiza os três conceitos anunciados, mas não substitui a explicação completa do professor nem confirma todos os exemplos apresentados no vídeo.
