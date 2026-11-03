# Modelo OSI — As 7 Camadas de Rede

## 1. Introdução

O **Modelo OSI (Open Systems Interconnection)** é um modelo de referência criado pela ISO (International Organization for Standardization) para padronizar a comunicação entre diferentes sistemas e dispositivos em uma rede.

Ele divide o processo de comunicação em **7 camadas**, cada uma com responsabilidades específicas.

O objetivo é facilitar o entendimento, a implementação e a identificação de problemas nas redes de computadores.

## 2. As 7 camadas do Modelo OSI

| Camada | Nome | Principal função |
|---|---|---|
| 7 | Aplicação | Oferece serviços de rede aos aplicativos. |
| 6 | Apresentação | Formata, codifica, comprime e criptografa dados. |
| 5 | Sessão | Gerencia sessões de comunicação. |
| 4 | Transporte | Controla a comunicação entre dispositivos e a entrega dos dados. |
| 3 | Rede | Realiza o endereçamento lógico e o roteamento. |
| 2 | Enlace de Dados | Organiza os dados em quadros e controla a comunicação no enlace. |
| 1 | Física | Transmite os bits pelo meio físico. |

## 3. Explicação de cada camada

### Camada 7 — Aplicação (Application)

É a camada mais próxima do usuário. Ela fornece serviços de rede utilizados pelos aplicativos.

**Exemplos de protocolos:**
- HTTP e HTTPS — acesso a páginas web.
- FTP — transferência de arquivos.
- SMTP — envio de e-mails.
- DNS — resolução de nomes de domínio.

**Exemplo prático:** quando acessamos um site pelo navegador, utilizamos serviços relacionados à camada de aplicação.

### Camada 6 — Apresentação (Presentation)

É responsável por preparar os dados para que os sistemas consigam interpretá-los corretamente.

**Principais funções:**
- Conversão e formatação de dados.
- Criptografia e descriptografia.
- Compressão e descompressão.

**Exemplos:**
- UTF-8 — codificação de caracteres.
- JPEG — formato de imagem.
- PNG — formato de imagem.
- TLS — segurança e criptografia, associado a esta camada no modelo conceitual.

**Exemplo prático:** converter dados para um formato que possa ser interpretado pelo sistema de destino.

### Camada 5 — Sessão (Session)

Responsável por estabelecer, gerenciar e encerrar sessões de comunicação entre aplicações.

**Principais funções:**
- Estabelecimento de sessões.
- Manutenção da comunicação.
- Encerramento de sessões.
- Sincronização e recuperação de diálogos.

**Exemplo prático:** controlar uma sessão de comunicação entre dois sistemas durante uma troca de informações.

### Camada 4 — Transporte (Transport)

Responsável pela comunicação entre os processos de origem e destino, organizando a entrega dos dados.

**Principais funções:**
- Segmentação e remontagem dos dados.
- Controle de fluxo.
- Controle de erros.
- Multiplexação por portas.

**Principais protocolos:**

**TCP (Transmission Control Protocol)**
- Comunicação orientada à conexão.
- Confirmação de recebimento.
- Controle de entrega e retransmissão.
- Maior confiabilidade.

**UDP (User Datagram Protocol)**
- Comunicação sem conexão.
- Menor sobrecarga.
- Não garante entrega ou ordenação dos dados.

**Exemplo prático:** o TCP é utilizado em diversas comunicações que exigem entrega confiável, enquanto o UDP é comum em aplicações de tempo real.

### Camada 3 — Rede (Network)

Responsável pelo endereçamento lógico e pela escolha dos caminhos que os pacotes percorrem entre redes diferentes.

**Principais funções:**
- Endereçamento IP.
- Roteamento de pacotes.
- Encaminhamento entre redes.

**Exemplos:**
- IPv4.
- IPv6.
- ICMP.
- Roteadores.

**Exemplo prático:** quando um computador acessa um servidor localizado em outra rede, a camada de rede participa do encaminhamento dos pacotes até o destino.

### Camada 2 — Enlace de Dados (Data Link)

Responsável pela comunicação entre dispositivos conectados ao mesmo enlace de rede.

**Principais funções:**
- Organização dos dados em quadros (frames).
- Endereçamento físico por MAC.
- Detecção de erros no enlace.
- Controle de acesso ao meio.

**Exemplos:**
- Ethernet (IEEE 802.3).
- Wi-Fi (IEEE 802.11).
- Switches.
- Endereços MAC.

**Exemplo prático:** um switch Ethernet utiliza informações de endereços MAC para encaminhar quadros dentro de uma rede local.

### Camada 1 — Física (Physical)

É a camada responsável pela transmissão dos bits através do meio físico.

**Principais elementos:**
- Cabos de rede.
- Fibra óptica.
- Conectores.
- Sinais elétricos, ópticos e de rádio.
- Repetidores e hubs.

**Exemplo prático:** quando os dados são transmitidos por um cabo Ethernet, os bits são representados por sinais físicos que percorrem o meio de transmissão.

## 4. Encapsulamento de dados

Quando uma informação é enviada pela rede, ela passa pelas camadas do modelo OSI, recebendo informações de controle em cada etapa.

Esse processo é chamado de **encapsulamento**.

Na transmissão, o processo ocorre da camada 7 até a camada 1.

Na recepção, ocorre o processo inverso, chamado de **desencapsulamento**, da camada 1 até a camada 7.

### Unidades de dados (PDU)

| Camada | Unidade de dados |
|---|---|
| Aplicação, Apresentação e Sessão | Dados |
| Transporte | Segmento (TCP) / Datagrama (UDP) |
| Rede | Pacote |
| Enlace de Dados | Quadro (Frame) |
| Física | Bits |

## 5. Equipamentos associados às camadas

| Camada | Exemplos |
|---|---|
| 7 — Aplicação | Proxy de aplicação, gateway de aplicação |
| 6 — Apresentação | Funções de codificação e criptografia |
| 5 — Sessão | Funções de gerenciamento de sessão |
| 4 — Transporte | Firewall com inspeção de portas, balanceadores |
| 3 — Rede | Roteadores |
| 2 — Enlace | Switches e bridges |
| 1 — Física | Hubs, repetidores e cabos |

**Observação:** os equipamentos modernos podem operar em várias camadas. Essa tabela apresenta associações didáticas, não limitações rígidas.

## 6. Como memorizar as camadas

Da camada 7 até a camada 1:

1. Aplicação
2. Apresentação
3. Sessão
4. Transporte
5. Rede
6. Enlace de Dados
7. Física

Uma forma de memorizar é associar cada camada à sua principal responsabilidade:

- Aplicação: serviços.
- Apresentação: formato.
- Sessão: comunicação.
- Transporte: entrega.
- Rede: caminhos.
- Enlace: quadros e MAC.
- Física: bits.

## 7. Por que o Modelo OSI é importante?

O Modelo OSI ajuda profissionais de TI a:

- Entender como ocorre a comunicação em redes.
- Identificar em qual camada um problema pode estar.
- Compreender a função dos protocolos de rede.
- Estudar roteadores, switches e outros equipamentos.
- Aprender conceitos fundamentais de infraestrutura e segurança.

## 8. Conclusão

O Modelo OSI é um dos principais fundamentos para compreender redes de computadores.

Conhecer suas sete camadas facilita o aprendizado de endereçamento IP, protocolos, roteamento, redes sem fio e segurança da informação.

**Próximo assunto:** Endereçamento IP — máscaras de sub-rede, gateway, CIDR e sub-redes.
