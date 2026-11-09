# Aula — Principais Protocolos e Equipamentos nas Camadas do Modelo OSI

## Introdução

O Modelo OSI divide a comunicação em redes em sete camadas. Cada camada possui funções específicas e utiliza protocolos e equipamentos para permitir a comunicação entre dispositivos.

## 1. Camada Física (Physical)

**Função:** transmitir bits (0 e 1) por meio de um meio físico.

- **Protocolos e padrões:** Ethernet PHY, USB, Bluetooth PHY e padrões IEEE 802.11 PHY.
- **Equipamentos:** cabos, conectores, repetidores e hubs.
- **Unidade de dados:** bits.

## 2. Camada de Enlace (Data Link)

**Função:** organizar os bits em quadros (frames) e controlar a comunicação entre dispositivos conectados ao mesmo enlace.

- **Protocolos e padrões:** Ethernet (IEEE 802.3), Wi-Fi (IEEE 802.11), PPP e HDLC.
- **Equipamentos:** switches e bridges.
- **Identificação:** endereço MAC.
- **Unidade de dados:** quadros (frames).

## 3. Camada de Rede (Network)

**Função:** realizar o endereçamento lógico e escolher caminhos para que os pacotes cheguem ao destino em outras redes.

- **Protocolos:** IPv4, IPv6, ICMP e IPsec.
- **Equipamentos:** roteadores.
- **Identificação:** endereço IP.
- **Unidade de dados:** pacotes.

## 4. Camada de Transporte (Transport)

**Função:** permitir a comunicação entre aplicações em dispositivos diferentes, utilizando portas para identificar os serviços.

- **Protocolos:** TCP e UDP.
- **Identificação:** números de portas.
- **Unidade de dados:** segmentos (TCP) e datagramas (UDP).

**TCP:** oferece comunicação confiável, com controle de entrega e ordenação dos dados.

**UDP:** possui menor sobrecarga e não garante entrega ou ordenação.

## 5. Camada de Sessão (Session)

**Função:** estabelecer, gerenciar e encerrar sessões de comunicação entre aplicações.

- **Exemplos de protocolos e mecanismos associados:** RPC e NetBIOS.
- **Responsabilidade:** controlar o diálogo entre aplicações e a continuidade da sessão.

## 6. Cam
