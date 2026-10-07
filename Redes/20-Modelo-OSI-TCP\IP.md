# 🌐 Modelos OSI e TCP/IP

## 📚 Introdução

Para entender como os dispositivos se comunicam em uma rede, existem modelos que organizam as diferentes funções envolvidas nessa comunicação.

Os dois modelos mais importantes estudados em redes são:

- **Modelo OSI**
- **Modelo TCP/IP**

Eles dividem a comunicação em camadas, permitindo organizar e compreender melhor o funcionamento das redes.

---

# 🧱 Modelo OSI

## O que é?

O **Modelo OSI (Open Systems Interconnection)** é um modelo de referência criado para organizar a comunicação de redes em **7 camadas**.

Cada camada possui responsabilidades específicas.

A ideia é dividir um processo complexo em partes menores e mais fáceis de entender.

---

# 7️⃣ As 7 camadas do Modelo OSI

| Nº | Camada | Função principal |
|---:|---|---|
| 7 | Aplicação | Serviços de rede utilizados pelas aplicações |
| 6 | Apresentação | Formatação, tradução, criptografia e compressão |
| 5 | Sessão | Estabelecimento e gerenciamento das sessões |
| 4 | Transporte | Comunicação entre processos, confiabilidade e portas |
| 3 | Rede | Endereçamento lógico e roteamento |
| 2 | Enlace | Comunicação local, MAC e frames |
| 1 | Física | Transmissão de bits e sinais |

---

## 7. Aplicação

É a camada mais próxima das aplicações.

Ela fornece serviços de rede utilizados pelos programas.

### Exemplos

- HTTP
- HTTPS
- DNS
- FTP
- SMTP

### Exemplo

Quando um navegador acessa:

```text
https://www.exemplo.com
```

protocolos da camada de aplicação participam da comunicação.

> A camada de aplicação não significa simplesmente "a tela do programa". Ela está relacionada aos protocolos e serviços utilizados pelas aplicações para comunicação em rede.

---

## 6. Apresentação

Está relacionada à forma como os dados são representados.

Pode envolver:

- Formatação
- Tradução
- Criptografia
- Descriptografia
- Compressão
- Descompressão

A ideia é permitir que os dados possam ser interpretados corretamente entre diferentes sistemas.

---

## 5. Sessão

Responsável pelo gerenciamento das sessões de comunicação entre aplicações.

Pode envolver:

- Estabelecimento de uma sessão
- Manutenção da sessão
- Controle da comunicação
- Encerramento da sessão

---

## 4. Transporte

Responsável pela comunicação entre processos/aplicações.

Entre suas funções estão:

- Segmentação dos dados
- Controle de fluxo
- Controle da comunicação
- Confiabilidade, dependendo do protocolo
- Utilização de portas

### Principais protocolos

```text
TCP
UDP
```

### TCP

O TCP oferece mecanismos para uma comunicação mais confiável.

Características:

- Entrega confiável
- Ordenação dos dados
- Retransmissão
- Controle de fluxo
- Controle de congestionamento

### UDP

O UDP possui uma estrutura mais simples e menor sobrecarga.

Não oferece as mesmas garantias de entrega e ordenação do TCP.

---

## 🔢 Portas

As portas ajudam a identificar serviços/processos envolvidos na comunicação.

Exemplo:

```text
192.168.1.10:8080
```

Nesse exemplo:

```text
192.168.1.10 → IP
8080         → porta
```

---

## 3. Rede

Responsável principalmente pelo **endereçamento lógico e roteamento**.

O principal protocolo é:

```text
IP
```

### IPv4

```text
192.168.1.10
```

### IPv6

```text
2001:db8::1
```

### Equipamento associado

**Roteador (Router)**

O roteador utiliza informações de endereçamento IP para encaminhar pacotes entre redes.

---

## 2. Enlace

Responsável pela comunicação dentro de um determinado enlace/rede local.

Entre seus conceitos estão:

- Endereço MAC
- Frames
- Comunicação local
- Controle de acesso ao meio

### Equipamento associado

**Switch**

O switch utiliza principalmente endereços MAC para encaminhar frames dentro da rede local.

### Exemplo de MAC

```text
AA:BB:CC:DD:EE:FF
```

---

## 1. Física

É responsável pela transmissão dos bits através do meio físico.

Exemplos:

- Cabos de rede
- Fibra óptica
- Ondas de rádio
- Sinais elétricos
- Sinais ópticos

---

# 📦 Encapsulamento no Modelo OSI

Durante o envio, cada camada pode adicionar informações necessárias à comunicação.

Uma representação simplificada:

```text
Dados
  ↓
Segmento
  ↓
Pacote
  ↓
Frame
  ↓
Bits
```

| Camada | Unidade de dados |
|---|---|
| Aplicação | Dados |
| Transporte | Segmento / Datagrama |
| Rede | Pacote |
| Enlace | Frame |
| Física | Bits |

No destino ocorre o processo inverso:

```text
Bits
  ↓
Frame
  ↓
Pacote
  ↓
Segmento/Datagrama
  ↓
Dados
```

Esse processo é chamado de **desencapsulamento**.

---

# 🌎 Modelo TCP/IP

## O que é?

O **modelo TCP/IP** é uma arquitetura de protocolos utilizada como base para a comunicação na Internet.

Diferentemente do OSI, que possui **7 camadas**, o modelo TCP/IP tradicionalmente é apresentado com **4 camadas**.

```text
4 - Aplicação
3 - Transporte
2 - Internet
1 - Acesso à Rede
```

---

# 🧱 As 4 camadas do TCP/IP

| Nº | Camada TCP/IP | Função |
|---:|---|---|
| 4 | Aplicação | Serviços e protocolos utilizados pelas aplicações |
| 3 | Transporte | Comunicação entre processos |
| 2 | Internet | Endereçamento e roteamento |
| 1 | Acesso à Rede | Comunicação com a rede e meio físico |

---

# 4️⃣ Camada de Aplicação

É responsável pelos protocolos utilizados diretamente pelas aplicações.

Exemplos:

- HTTP
- HTTPS
- DNS
- FTP
- SMTP

No modelo TCP/IP, funções que aparecem separadas nas camadas:

```text
Aplicação
Apresentação
Sessão
```

do modelo OSI são normalmente agrupadas na camada:

```text
Aplicação
```

---

# 3️⃣ Camada de Transporte

É responsável pela comunicação entre processos.

Principais protocolos:

```text
TCP
UDP
```

Também estão relacionados a essa camada conceitos como:

- Portas
- Segmentação
- Controle de fluxo
- Confiabilidade, no caso do TCP

---

# 2️⃣ Camada de Internet

É responsável principalmente pelo endereçamento lógico e pelo roteamento dos pacotes.

Principal protocolo:

```text
IP
```

Exemplos:

```text
IPv4
IPv6
```

Essa camada corresponde aproximadamente à:

```text
Camada 3 - Rede
```

do modelo OSI.

---

# 1️⃣ Camada de Acesso à Rede

Está relacionada à comunicação com a rede e ao meio utilizado para transmitir os dados.

Envolve conceitos relacionados a:

- Ethernet
- Wi-Fi
- MAC
- Frames
- Meios físicos
- Transmissão de dados

No modelo OSI, essas funções são divididas principalmente entre:

```text
Camada 2 - Enlace
Camada 1 - Física
```

---

# 🔄 OSI x TCP/IP

A relação simplificada entre os dois modelos pode ser representada assim:

```text
              MODELO OSI              MODELO TCP/IP

          7 - Aplicação
          6 - Apresentação  ────────►  4 - Aplicação
          5 - Sessão

          4 - Transporte    ────────►  3 - Transporte

          3 - Rede          ────────►  2 - Internet

          2 - Enlace
          1 - Física        ────────►  1 - Acesso à Rede
```

Ou em tabela:

| Modelo OSI | Modelo TCP/IP |
|---|---|
| 7. Aplicação | 4. Aplicação |
| 6. Apresentação | 4. Aplicação |
| 5. Sessão | 4. Aplicação |
| 4. Transporte | 3. Transporte |
| 3. Rede | 2. Internet |
| 2. Enlace | 1. Acesso à Rede |
| 1. Física | 1. Acesso à Rede |

---

# 🧠 Diferença principal

A maneira mais simples de lembrar:

```text
OSI
↓
7 camadas
↓
Modelo de referência

TCP/IP
↓
4 camadas
↓
Arquitetura baseada nos protocolos utilizados na Internet
```

O OSI separa algumas funções que o TCP/IP agrupa.

Por exemplo:

```text
OSI:

Aplicação
Apresentação
Sessão

        ↓

TCP/IP:

Aplicação
```

E:

```text
OSI:

Enlace
Física

        ↓

TCP/IP:

Acesso à Rede
```

---

# 🌐 Exemplo: acessando um site

Imagine que você digite:

```text
https://www.exemplo.com
```

Uma visão simplificada usando o modelo TCP/IP:

```text
┌─────────────────────────────┐
│ Aplicação                   │
│ HTTP / HTTPS / DNS          │
├─────────────────────────────┤
│ Transporte                  │
│ TCP / UDP / Portas          │
├─────────────────────────────┤
│ Internet                    │
│ IP / Roteamento             │
├─────────────────────────────┤
│ Acesso à Rede               │
│ Ethernet / Wi-Fi / MAC      │
└─────────────────────────────┘
```

Os dados passam pelas camadas durante o envio.

No destino, ocorre o processo inverso.

---

# 🔗 Relacionando com o que já estudei

Os modelos ajudam a organizar vários assuntos que já apareceram durante o estudo de redes.

```text
MODELO OSI

7 - Aplicação
    ├── HTTP
    ├── HTTPS
    ├── DNS
    ├── FTP
    └── SMTP

6 - Apresentação
    ├── Formatação
    ├── Criptografia
    └── Compressão

5 - Sessão
    └── Gerenciamento de sessões

4 - Transporte
    ├── TCP
    ├── UDP
    └── Portas

3 - Rede
    ├── IP
    ├── IPv4
    ├── IPv6
    └── Roteamento

2 - Enlace
    ├── MAC
    ├── Frames
    └── Switch

1 - Física
    ├── Cabos
    ├── Fibra óptica
    └── Rádio
```

---

# 🧩 Uma forma simples de pensar

Quando um computador acessa um servidor:

```text
APLICAÇÃO
"O que quero fazer?"

       ↓

TRANSPORTE
"Qual processo/serviço deve receber?"

       ↓

REDE / INTERNET
"Para qual IP devo enviar?"

       ↓

ENLACE
"Como envio dentro desta rede?"

       ↓

FÍSICA
"Como os bits serão transmitidos?"
```

Essa visão ajuda bastante a conectar os assuntos.

---

# 💻 Relação com programação

O estudo desses modelos será útil posteriormente no desenvolvimento.

Por exemplo:

```text
Frontend
   ↓
HTTP / HTTPS
   ↓
TCP / UDP
   ↓
IP
   ↓
Ethernet / Wi-Fi
   ↓
Rede
```

Quando você começar a estudar:

- Java
- Spring Boot
- APIs REST
- HTTP
- HTTPS
- Banco de dados
- Front-end
- WebSockets
- Microsserviços

esses conceitos de redes voltarão a aparecer.

Um exemplo que você verá futuramente:

```text
http://localhost:8080
```

Onde:

```text
localhost → máquina local
8080      → porta
HTTP      → protocolo de aplicação
```

---

# 📝 Perguntas para revisão

Depois de estudar, tente responder sem consultar as anotações:

### Modelo OSI

1. O que é o Modelo OSI?
2. Quantas camadas ele possui?
3. Qual a função de cada camada?
4. Em qual camada encontramos o IP?
5. Em qual camada encontramos o MAC?
6. Em qual camada ficam TCP e UDP?
7. Em qual camada ficam as portas?
8. Em qual camada normalmente encontramos HTTP e HTTPS?
9. O que é encapsulamento?
10. O que é desencapsulamento?

### Modelo TCP/IP

11. Quantas camadas possui o modelo TCP/IP tradicional?
12. Quais são as quatro camadas?
13. Qual é a função da camada Internet?
14. Qual é a função da camada de Transporte?
15. Qual é a função da camada de Aplicação?
16. Qual é a função da camada de Acesso à Rede?

### Comparação

17. Qual é a principal diferença entre OSI e TCP/IP?
18. Quais camadas do OSI são agrupadas na camada de Aplicação do TCP/IP?
19. Quais camadas do OSI correspondem aproximadamente à camada de Acesso à Rede do TCP/IP?
20. Por que estudar os dois modelos?

---

# 🎯 O que realmente preciso memorizar?

Não é necessário decorar tudo imediatamente.

### 🟢 Prioridade alta

```text
OSI = 7 camadas

TCP/IP = 4 camadas
```

E saber relacionar:

```text
OSI                     TCP/IP

Aplicação ┐
           ├──────────► Aplicação
Apresentação
Sessão    ┘

Transporte ──────────► Transporte

Rede ────────────────► Internet

Enlace ┐
        ├────────────► Acesso à Rede
Física ┘
```

Também é importante saber:

```text
IP       → Rede / Internet
MAC      → Enlace / Acesso à Rede
TCP/UDP  → Transporte
Portas   → Transporte
HTTP     → Aplicação
HTTPS    → Aplicação
```

---

# 🧠 Resumo final

## Modelo OSI

```text
7 - Aplicação
6 - Apresentação
5 - Sessão
4 - Transporte
3 - Rede
2 - Enlace
1 - Física
```

## Modelo TCP/IP

```text
4 - Aplicação
3 - Transporte
2 - Internet
1 - Acesso à Rede
```

## Relação

```text
OSI                           TCP/IP

Aplicação
Apresentação                 → Aplicação
Sessão

Transporte                   → Transporte

Rede                         → Internet

Enlace
Física                       → Acesso à Rede
```

> **Modelo OSI:** divide a comunicação em 7 camadas para facilitar a organização e o entendimento.

> **Modelo TCP/IP:** organiza a comunicação em uma arquitetura mais enxuta, baseada nos protocolos que formam a base da comunicação em redes, especialmente na Internet.

---

# 📌 Mentalidade para guardar

Não pense no OSI e TCP/IP como duas redes diferentes.

Pense neles como **duas formas de organizar e explicar as funções envolvidas na comunicação de redes**.

```text
              COMUNICAÇÃO EM REDE
                       │
          ┌────────────┴────────────┐
          │                         │
       MODELO OSI               MODELO TCP/IP
       7 camadas                 4 camadas
          │                         │
          └──────────┬──────────────┘
                     │
              MESMO OBJETIVO:
          entender a comunicação
               entre sistemas
```
