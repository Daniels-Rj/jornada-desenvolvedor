# Tipos de Comunicação em Redes e Endereço MAC

## 1. O que é comunicação em uma rede?

Em uma rede de computadores, **comunicação** é o processo pelo qual dispositivos trocam informações entre si.

Exemplos de dispositivos que podem participar dessa comunicação:

- Computadores
- Smartphones
- Impressoras
- Roteadores
- Switches
- Servidores
- Smart TVs
- Consoles
- Câmeras
- Dispositivos IoT

Quando um dispositivo envia dados para outro, precisamos saber:

- Quem está enviando;
- Quem deve receber;
- Por onde os dados devem passar.

É aí que entram conceitos como:

- **MAC**
- **IP**
- **Unicast**
- **Broadcast**
- **Multicast**

---

# 2. Tipos de comunicação

Existem diferentes formas de um dispositivo enviar dados dentro de uma rede.

Os principais tipos estudados são:

```text
Comunicação
├── Unicast
├── Broadcast
└── Multicast
```

---

# 3. Unicast

**Unicast** é uma comunicação de **um dispositivo para outro dispositivo específico**.

```text
Computador A
     │
     │
     ▼
Computador B
```

Somente o destinatário escolhido deve receber aquela comunicação.

### Exemplo

Imagine que seu computador:

```text
IP: 192.168.1.10
```

quer enviar um arquivo para:

```text
IP: 192.168.1.20
```

A comunicação é:

```text
192.168.1.10
      │
      │ dados
      ▼
192.168.1.20
```

Isso é **Unicast**.

### Exemplos do cotidiano

Quando você:

- acessa um site;
- envia uma mensagem para uma pessoa;
- baixa um arquivo de um servidor;
- acessa uma API;
- conecta seu computador a um servidor de jogo;

normalmente existe comunicação **Unicast** envolvida.

---

# 4. Broadcast

**Broadcast** significa que uma mensagem é enviada para **todos os dispositivos de determinado domínio de broadcast**.

Imagine uma rede:

```text
              ┌── PC 1
              │
              ├── PC 2
              │
PC 1 ─────────┼── PC 3
              │
              ├── Celular
              │
              └── Impressora
```

Se um dispositivo envia um Broadcast:

```text
          BROADCAST
              │
      ┌───────┼───────┐
      ▼       ▼       ▼
     PC 1    PC 2    PC 3
              │
              ▼
           Celular
```

Todos os dispositivos pertencentes àquele domínio recebem a transmissão.

---

## 4.1 Exemplo: DHCP

Um exemplo muito importante de Broadcast acontece quando um dispositivo entra em uma rede e ainda **não possui um endereço IP**.

Imagine que você conecta seu notebook ao Wi-Fi.

Ele precisa descobrir:

> "Existe algum servidor DHCP que possa me fornecer um endereço IP?"

Ele pode iniciar o processo utilizando uma mensagem de Broadcast.

De forma simplificada:

```text
Notebook
   │
   │ "Tem algum servidor DHCP aqui?"
   │
   ▼
BROADCAST
   │
   ├── Celular
   ├── TV
   ├── Computador
   └── Roteador/DHCP
                │
                ▼
          "Eu sou o DHCP"
```

O DHCP pode fornecer informações como:

- Endereço IP;
- Máscara de sub-rede;
- Gateway;
- Servidor DNS.

---

# 5. Multicast

**Multicast** fica entre Unicast e Broadcast.

Em vez de enviar:

```text
1 → 1
```

ou:

```text
1 → todos
```

temos:

```text
1 → grupo específico
```

Imagine:

```text
              ┌── PC 1
              │
Servidor ─────┼── PC 2
              │
              ├── PC 3
              │
              └── PC 4
```

Se PC 1 e PC 3 pertencem a determinado grupo multicast:

```text
              ┌── PC 1 ✓
              │
Servidor ─────┼── PC 2
              │
              ├── PC 3 ✓
              │
              └── PC 4
```

A informação é enviada para **os membros daquele grupo**, e não para todos os dispositivos.

---

# 6. Comparação entre Unicast, Broadcast e Multicast

| Tipo | Comunicação | Exemplo conceitual |
|---|---|---|
| **Unicast** | 1 → 1 | Computador → servidor |
| **Broadcast** | 1 → todos | Descoberta DHCP |
| **Multicast** | 1 → grupo | Comunicação com grupo específico |

Uma maneira fácil de memorizar:

```text
UNICAST
1 ───────► 1

BROADCAST
1 ───────► TODOS

MULTICAST
1 ───────► GRUPO
```

---

# 7. O que é MAC?

**MAC** significa:

> **Media Access Control**

O endereço MAC é um identificador utilizado na comunicação de rede, principalmente na **camada de enlace**.

Ele está associado à interface de rede.

Por exemplo, seu computador pode possuir:

- uma interface Wi-Fi;
- uma interface Ethernet.

Cada interface pode possuir seu próprio endereço MAC.

---

# 8. Exemplo de endereço MAC

Um endereço MAC tradicionalmente é representado por **48 bits**, normalmente escritos em hexadecimal.

Exemplo:

```text
00:1A:2B:3C:4D:5E
```

Também podemos encontrar formatos como:

```text
00-1A-2B-3C-4D-5E
```

São apenas formas diferentes de representar o endereço.

---

# 9. Por que o MAC utiliza hexadecimal?

O endereço MAC tradicional possui **48 bits**.

Representar 48 bits diretamente seria pouco prático:

```text
000000000001101000101011001111000100110101011110
```

Por isso usamos hexadecimal:

```text
00:1A:2B:3C:4D:5E
```

Cada caractere hexadecimal representa **4 bits**.

Os símbolos possíveis são:

```text
0 1 2 3 4 5 6 7 8 9 A B C D E F
```

Como:

```text
1 hexadecimal = 4 bits
```

e o MAC possui:

```text
48 bits
```

temos:

```text
48 ÷ 4 = 12
```

Por isso um endereço MAC tradicional possui **12 caracteres hexadecimais**.

---

# 10. MAC não é a mesma coisa que IP

Essa diferença é extremamente importante.

## MAC

Está relacionado à comunicação na **rede local** e à camada de enlace.

Exemplo:

```text
00:1A:2B:3C:4D:5E
```

## IP

É um endereço lógico utilizado para identificar e localizar dispositivos em uma rede IP.

IPv4:

```text
192.168.1.10
```

IPv6:

```text
2001:db8::10
```

Podemos pensar inicialmente assim:

```text
MAC → identificação da interface na rede local

IP → endereçamento lógico para comunicação entre redes
```

> Essa é uma simplificação inicial. O funcionamento real das redes possui mais detalhes.

---

# 11. MAC e IP trabalhando juntos

Imagine:

```text
Computador A

IP:
192.168.1.10

MAC:
AA:AA:AA:AA:AA:AA
```

quer conversar com:

```text
Computador B

IP:
192.168.1.20

MAC:
BB:BB:BB:BB:BB:BB
```

O computador A sabe o **IP** do destino.

Mas, dentro da rede local Ethernet, ele também precisa descobrir o **MAC correspondente**.

No IPv4, um dos mecanismos utilizados para isso é o **ARP (Address Resolution Protocol)**.

---

# 12. ARP

O ARP permite descobrir:

> "Qual é o MAC correspondente a determinado endereço IPv4?"

Imagine:

```text
PC A

IP:
192.168.1.10

MAC:
AA:AA:AA:AA:AA:AA
```

Ele quer falar com:

```text
192.168.1.20
```

Mas ainda não conhece o MAC.

Então, simplificando:

```text
PC A
 │
 │ "Quem possui 192.168.1.20?"
 │
 ▼
Broadcast ARP
 │
 ├── PC 1
 ├── PC 2
 ├── PC 3
 └── PC B ✓
        │
        │ "Sou eu.
        │ Meu MAC é BB:BB:BB:BB:BB:BB"
        ▼
PC A aprende o MAC
```

Depois disso, pode enviar os quadros para o MAC correto.

---

# 13. Quadro e pacote

Na comunicação de redes, diferentes camadas trabalham com diferentes unidades de dados.

De forma simplificada:

```text
Aplicação
   ↓
Dados

Transporte
   ↓
Segmento / Datagrama

Rede
   ↓
Pacote

Enlace
   ↓
Quadro (Frame)

Física
   ↓
Bits
```

O **MAC** está principalmente associado ao **quadro (frame)** da camada de enlace.

O **IP** está associado ao **pacote** da camada de rede.

---

# 14. Exemplo completo de comunicação

Imagine que você acessa um servidor na Internet.

Seu computador possui:

```text
IP local:
192.168.1.10

MAC:
AA:AA:AA:AA:AA:AA
```

Seu roteador possui, por exemplo:

```text
IP local:
192.168.1.1

MAC:
RR:RR:RR:RR:RR:RR
```

Você quer acessar um servidor:

```text
203.0.113.50
```

Seu computador percebe que o destino está fora da sua rede local.

Então ele não precisa descobrir o MAC do servidor remoto.

Ele precisa entregar o quadro ao **próximo dispositivo da rede local**, normalmente o roteador/gateway.

Conceitualmente:

```text
Seu computador
      │
      │ Ethernet/Wi-Fi
      ▼
Roteador
      │
      │ Internet
      ▼
Outros roteadores
      │
      ▼
Servidor
```

Isso é uma das razões pelas quais **MAC e IP possuem funções diferentes**.

---

# 15. O MAC atravessa a Internet inteira?

**Não da forma como podemos imaginar inicialmente.**

O MAC é utilizado principalmente dentro do **segmento de rede local**.

Quando um pacote atravessa roteadores:

```text
PC
 ↓
Roteador 1
 ↓
Roteador 2
 ↓
Roteador 3
 ↓
Servidor
```

o pacote IP continua sendo encaminhado, mas os **quadros de enlace são reconstruídos a cada trecho**.

Uma simplificação útil:

```text
TRECHO 1

PC ─────────► Roteador 1

MAC:
PC → Roteador 1
```

```text
TRECHO 2

Roteador 1 ─────────► Roteador 2

MAC:
Roteador 1 → Roteador 2
```

```text
TRECHO 3

Roteador 2 ─────────► Roteador 3

MAC:
Roteador 2 → Roteador 3
```

Enquanto isso, o endereçamento IP participa do encaminhamento do pacote entre redes.

---

# 16. MAC e Switch

O **switch** trabalha principalmente na camada de enlace.

Ele utiliza endereços MAC para decidir por qual porta deve encaminhar um quadro.

Imagine:

```text
             Switch
          ┌────┼────┐
          │    │    │
         PC1  PC2  PC3
```

O switch pode aprender:

```text
MAC do PC1 → porta 1
MAC do PC2 → porta 2
MAC do PC3 → porta 3
```

Quando recebe um quadro destinado ao MAC do PC2, pode encaminhá-lo para a porta correspondente.

Isso reduz transmissões desnecessárias.

---

# 17. Broadcast e Switch

Quando um quadro é Broadcast dentro de um domínio de broadcast, o switch pode encaminhá-lo para várias portas.

Por isso, Broadcast não significa simplesmente:

> "O computador manda para todos os computadores existentes no mundo."

Significa:

> **A mensagem é destinada a todos os dispositivos dentro daquele domínio de broadcast.**

---

# 18. Domínio de Broadcast

Um **domínio de broadcast** é, simplificando, o conjunto de dispositivos que pode receber determinado Broadcast de camada 2.

Um roteador normalmente separa domínios de broadcast.

Exemplo:

```text
          ROTEADOR
          /      \
         /        \
    Rede A        Rede B
   PC1 PC2       PC3 PC4
```

Um Broadcast da Rede A não é simplesmente propagado para a Rede B pelo roteador.

Isso ajuda a limitar o alcance dos Broadcasts.

---

# 19. Resumo dos principais conceitos

```text
COMUNICAÇÃO
│
├── Unicast
│   └── 1 → 1
│
├── Broadcast
│   └── 1 → todos dentro do domínio
│
└── Multicast
    └── 1 → grupo
```

```text
MAC
│
├── Media Access Control
├── 48 bits (MAC tradicional)
├── normalmente representado em hexadecimal
├── associado à interface de rede
└── utilizado principalmente na camada de enlace
```

```text
IP
│
├── Endereço lógico
├── IPv4 = 32 bits
├── IPv6 = 128 bits
└── utilizado no encaminhamento IP
```

```text
ARP
└── IPv4 → descoberta do MAC correspondente
```

```text
SWITCH
└── utiliza MAC para encaminhar quadros
```

```text
ROTEADOR
└── conecta redes diferentes e encaminha pacotes IP
```

---

# 20. A diferença que você precisa guardar

Se lembrar apenas de uma coisa desta aula, lembre:

```text
MAC
↓
"Qual interface de rede é o destino neste trecho da rede local?"

IP
↓
"Qual é o endereço lógico do destino e para qual rede devo encaminhar?"
```

E:

```text
UNICAST
1 → 1

BROADCAST
1 → TODOS

MULTICAST
1 → GRUPO
```

---

# 21. Como isso se conecta ao que já foi estudado

Os conceitos de redes começam a se encaixar:

```text
                  REDES
                    │
        ┌───────────┼───────────┐
        ↓           ↓           ↓
       MAC          IP         DNS
        │           │           │
        ↓           ↓           ↓
     Rede local   Roteamento   Nome → IP
        │           │
        └──────┬────┘
               ↓
            Pacotes
               ↓
          Roteadores
               ↓
            Internet
```

A Internet não é simplesmente:

> "Um computador conectado ao outro."

Existe uma enorme quantidade de mecanismos trabalhando juntos:

```text
Aplicação
   ↓
HTTP/HTTPS
   ↓
TCP/UDP
   ↓
IP
   ↓
MAC
   ↓
Wi-Fi / Ethernet / Fibra
   ↓
Roteadores e switches
   ↓
Internet
```

---

# 22. Relação com programação

Esses conceitos de redes serão importantes quando começarmos a estudar programação.

Por exemplo:

```text
Java
 ↓
HTTP
 ↓
API REST
 ↓
IP
 ↓
TCP
 ↓
Ethernet/Wi-Fi
```

Quando você futuramente construir um sistema **Full Stack**, poderá ter:

```text
┌──────────────────────────┐
│       FRONT-END          │
│ HTML + CSS + JavaScript  │
└────────────┬─────────────┘
             │
             │ HTTP/HTTPS
             ▼
┌──────────────────────────┐
│        BACK-END          │
│ Java + Spring Boot       │
│ API REST                 │
└────────────┬─────────────┘
             │
             │ SQL
             ▼
┌──────────────────────────┐
│      BANCO DE DADOS      │
│ MySQL / PostgreSQL       │
└──────────────────────────┘
```

Por baixo de tudo isso, a comunicação depende das redes que você está estudando agora.

---

# 23. Conclusão

Nesta aula, aprendemos que os dispositivos podem se comunicar de diferentes maneiras:

- **Unicast:** um dispositivo para outro;
- **Broadcast:** um dispositivo para todos dentro de determinado domínio;
- **Multicast:** um dispositivo para um grupo específico.

Também vimos que:

- **MAC** identifica uma interface de rede no contexto da comunicação de enlace;
- **IP** fornece endereçamento lógico para comunicação entre redes;
- **ARP** permite descobrir o MAC associado a um IPv4 na rede local;
- **Switches** utilizam MACs para encaminhar quadros;
- **Roteadores** encaminham pacotes entre redes;
- MAC e IP possuem funções diferentes e trabalham juntos;
- O MAC não é utilizado como endereço de ponta a ponta através de toda a Internet;
- A comunicação na Internet envolve várias camadas trabalhando em conjunto.

### Resumo mental

```text
MAC → comunicação no enlace / rede local
IP  → comunicação entre redes
ARP → IPv4 → MAC
Switch → MAC
Router → IP

Unicast   → 1
Broadcast → todos
Multicast → grupo
```

> **Ideia principal:** redes funcionam através da cooperação de várias tecnologias e camadas. O MAC ajuda a entregar quadros no trecho local, enquanto o IP permite que os pacotes sejam encaminhados entre diferentes redes.
