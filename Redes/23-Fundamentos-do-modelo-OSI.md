# Fundamentos do Modelo OSI

## 1. O que é o Modelo OSI?

O **Modelo OSI (Open Systems Interconnection)** é um modelo de referência que organiza e padroniza a comunicação entre diferentes dispositivos e sistemas em uma rede de computadores.

Ele foi desenvolvido pela ISO (International Organization for Standardization) e divide a comunicação em **7 camadas**, cada uma com uma função específica.

O modelo facilita o entendimento de como os dados são transmitidos e ajuda a identificar problemas nas redes.

## 2. As 7 camadas do Modelo OSI

| Número | Camada | Função principal |
|---|---|---|
| 7 | Aplicação | Oferece serviços de rede aos aplicativos. |
| 6 | Apresentação | Formata, codifica, comprime e criptografa dados. |
| 5 | Sessão | Gerencia as sessões de comunicação. |
| 4 | Transporte | Controla a comunicação e a entrega dos dados. |
| 3 | Rede | Trabalha com endereçamento IP e roteamento. |
| 2 | Enlace de Dados | Trabalha com quadros e endereços MAC. |
| 1 | Física | Transmite os bits pelo meio físico. |

## 3. Entendendo as camadas

### Camada 7 — Aplicação

É a camada mais próxima do usuário. Fornece serviços de rede utilizados pelos aplicativos.

**Exemplos:**
- HTTP e HTTPS.
- FTP.
- SMTP.
- DNS.

**Exemplo prático:** acessar um site pelo navegador.

### Camada 6 — Apresentação

Prepara os dados para que possam ser interpretados corretamente pelo sistema de destino.

**Principais funções:**
- Formatação dos dados.
- Codificação.
- Criptografia.
- Compressão.

**Exemplo prático:** converter informações para um formato que o sistema de destino consiga interpretar.

### Camada 5 — Sessão

Gerencia a comunicação entre aplicações, estabelecendo, mantendo e encerrando sessões.

**Principais funções:**
- Estabelecer sessões.
- Manter a comunicação.
- Encerrar sessões.
- Sincronizar a troca de informações.

**Exemplo prático:** manter uma sessão de comunicação ativa entre dois
