# Endereço IP, Máscara de Sub-rede, Gateway, DNS e MAC

## 1. Introdução

Para que dispositivos consigam se comunicar em uma rede, várias informações diferentes trabalham em conjunto.

Entre as principais estão:

- **Endereço IP**
- **Máscara de sub-rede**
- **Gateway**
- **Servidor DNS**
- **Endereço MAC**

Apesar de todos estarem relacionados à comunicação em redes, **cada um possui uma função diferente**.

---

# 2. Visão geral

| Conceito | Função principal | Exemplo |
|---|---|---|
| **IP** | Endereçamento lógico do dispositivo | `192.168.1.10` |
| **Máscara de sub-rede** | Define a parte da rede e a parte do host | `255.255.255.0` |
| **Gateway** | Saída da rede local para outras redes | `192.168.1.1` |
| **DNS** | Traduz nomes de domínio em endereços IP | `google.com → IP` |
| **MAC** | Identifica uma interface de rede no enlace | `AA:BB:CC:DD:EE:FF` |

---

# 3. Endereço IP

O **IP (Internet Protocol)** é utilizado para o **endereçamento lógico** dos dispositivos em uma rede IP.

Exemplo:

```text
Computador
IP: 192.168.1.10
```

Outro dispositivo:

```text
Celular
IP: 192.168.1.11
```

Roteador:

```text
IP: 192.168.1.1
```

Podemos visualizar:

```text
              ROTEADOR
            192.168.1.1
                 │
       ┌─────────┼─────────┐
       │         │         │
       ▼         ▼         ▼
      PC       Celular     TV
 .1.10          .1.11     .1.12
```

O endereço IP permite que os dispositivos sejam **endereçados logicamente dentro de uma rede**.

---

# 4. IPv4

Um endereço IPv4 possui **32 bits** e normalmente é representado por quatro números separados por pontos.

Exemplo:

```text
192.168.1.10
```

Cada parte pode variar de:

```text
0 até 255
```

Exemplo em binário:

```text
192.168.1.10

192 = 11000000
168 = 10101000
1   = 00000001
10  = 00001010
```

Portanto:

```text
192.168.1.10
```

é uma representação mais fácil de ler do endereço binário.

---

# 5. Endereço IP pode mudar

O IP não precisa ser permanentemente o mesmo.

Em uma rede doméstica, por exemplo, o roteador normalmente utiliza **DHCP** para distribuir endereços IP aos dispositivos.

Um computador pode receber:

```text
192.168.1.10
```

e posteriormente receber:

```text
192.168.1.15
```

Isso depende da configuração da rede e da concessão do endereço pelo DHCP.

---

# 6. Máscara de sub-rede

A **máscara de sub-rede** ajuda a determinar:

- qual parte do endereço IP representa a **rede**;
- qual parte representa o **host/dispositivo**.

Exemplo:

```text
IP:
192.168.1.10

Máscara:
255.255.255.0
```

Nesse caso, podemos representar de forma simplificada:

```text
192.168.1 . 10
──────────   ──
   REDE      HOST
```

A máscara:

```text
255.255.255 . 0
───────────   ─
    REDE     HOST
```

Indica que os três primeiros octetos pertencem à parte da rede e o último está disponível para identificação dos hosts.

---

# 7. Notação CIDR

A máscara também pode ser representada utilizando **CIDR**.

Por exemplo:

```text
255.255.255.0
```

equivale a:

```text
/24
```

Então podemos escrever:

```text
192.168.1.10/24
```

O `/24` significa que os primeiros **24 bits** pertencem à parte da rede.

---

# 8. Rede local

Com:

```text
IP:
192.168.1.10

Máscara:
255.255.255.0
```

a rede pode ser representada como:

```text
192.168.1.0/24
```

Outros dispositivos como:

```text
192.168.1.20
192.168.1.30
192.168.1.50
```

também pertencem a essa mesma rede.

Isso permite que o dispositivo determine se determinado destino está ou não na rede local.

---

# 9. Para que serve a máscara?

Imagine que:

```text
Computador:
192.168.1.10/24
```

quer falar com:

```text
192.168.1.20
```

Ele verifica se o destino pertence à mesma rede.

Como ambos estão em:

```text
192.168.1.0/24
```

o destino está na rede local.

Por outro lado, se quiser acessar:

```text
8.8.8.8
```

o destino não pertence à rede local.

Nesse caso, o computador normalmente precisa encaminhar o tráfego para o **gateway**.

---

# 10. Gateway

O **gateway** é, de forma simplificada, a **porta de saída da rede local para outras redes**.

Em redes domésticas, normalmente o gateway é o próprio roteador.

Exemplo:

```text
Computador
192.168.1.10
      │
      ▼
Gateway
192.168.1.1
      │
      ▼
Internet
```

Se o computador precisa se comunicar com um destino que está fora da rede local, ele normalmente envia o tráfego para o gateway.

---

# 11. Analogia do Gateway

Podemos imaginar uma rede local como um condomínio.

```text
Apartamento
     ↓
Condomínio
     ↓
Portão de saída
     ↓
Rua
     ↓
Cidade
```

O **gateway** seria semelhante ao portão de saída.

Dentro da rede local:

```text
PC → outro dispositivo da rede
```

Fora da rede:

```text
PC → Gateway → outras redes
```

---

# 12. DNS

**DNS** significa:

> **Domain Name System**

Sua principal função é realizar a resolução de nomes de domínio.

Nós preferimos utilizar nomes como:

```text
google.com
youtube.com
github.com
```

em vez de decorar endereços IP.

O DNS permite fazer a associação:

```text
Nome de domínio
      ↓
     DNS
      ↓
Endereço IP
```

De forma simplificada:

```text
google.com
     ↓
DNS
     ↓
IP do servidor
```

---

# 13. Exemplo de DNS

Quando você digita:

```text
www.exemplo.com
```

seu dispositivo precisa descobrir qual endereço IP está associado àquele nome.

O processo, de forma simplificada:

```text
Você digita:

www.exemplo.com
       │
       ▼
      DNS
       │
       ▼
Endereço IP
       │
       ▼
Servidor
```

Depois disso, o dispositivo pode estabelecer a comunicação com o destino.

---

# 14. DNS não é a Internet

É importante não confundir:

```text
DNS ≠ Internet
```

O DNS é um **sistema de resolução de nomes** utilizado pela Internet e por outras redes IP.

Ele ajuda a transformar nomes fáceis de lembrar em informações que podem ser utilizadas na comunicação.

---

# 15. Endereço MAC

**MAC** significa:

> **Media Access Control**

O endereço MAC está associado a uma **interface de rede** e é utilizado principalmente na comunicação da **camada de enlace**.

Exemplo:

```text
AA:BB:CC:DD:EE:FF
```

Um computador pode possuir diferentes interfaces de rede, como:

- Wi-Fi;
- Ethernet.

Cada interface pode possuir seu próprio endereço MAC.

Exemplo:

```text
Computador
│
├── Wi-Fi
│   └── MAC A
│
└── Ethernet
    └── MAC B
```

---

# 16. MAC não é o mesmo que IP

Essa é uma diferença fundamental.

### IP

É utilizado no **endereçamento lógico** da rede IP.

Exemplo:

```text
192.168.1.10
```

### MAC

Está associado à **interface de rede** e é utilizado principalmente no nível de enlace.

Exemplo:

```text
AA:BB:CC:DD:EE:FF
```

Podemos pensar inicialmente:

```text
IP
↓
Endereço lógico

MAC
↓
Endereço da interface no enlace local
```

---

# 17. MAC e IP trabalhando juntos

Imagine:

```text
Computador A

IP:
192.168.1.10

MAC:
AA:AA:AA:AA:AA:AA
```

e:

```text
Computador B

IP:
192.168.1.20

MAC:
BB:BB:BB:BB:BB:BB
```

O computador A sabe que quer falar com:

```text
192.168.1.20
```

Dentro da rede local IPv4, ele pode precisar descobrir qual MAC está associado a esse IP.

Para isso, pode utilizar o **ARP**.

---

# 18. ARP

**ARP (Address Resolution Protocol)** é utilizado em redes IPv4 para descobrir o endereço MAC associado a um endereço IPv4 na rede local.

Exemplo:

```text
PC A
IP: 192.168.1.10
MAC: AA:AA:AA:AA:AA:AA
```

Quer encontrar:

```text
192.168.1.20
```

Mas não sabe o MAC.

Pode enviar uma solicitação ARP:

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
 └── PC B
       │
       │ "Sou eu."
       │
       │ MAC:
       │ BB:BB:BB:BB:BB:BB
       ▼
PC A aprende o MAC
```

Depois disso, o dispositivo pode utilizar o MAC para a comunicação no enlace local.

---

# 19. Switch e MAC

O **switch** trabalha principalmente na camada de enlace.

Ele utiliza endereços MAC para encaminhar quadros para as portas apropriadas.

Exemplo:

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

Assim, quando recebe um quadro destinado ao PC2, pode encaminhá-lo pela porta correspondente.

---

# 20. Roteador e IP

O roteador trabalha principalmente na camada de rede e utiliza informações de IP para encaminhar pacotes entre redes.

Exemplo:

```text
Rede A
192.168.1.0/24
      │
      ▼
  Roteador
      │
      ▼
Rede B
10.0.0.0/24
```

O roteador conecta diferentes redes e decide para onde encaminhar os pacotes.

---

# 21. MAC não atravessa a Internet inteira

O endereço MAC é utilizado principalmente no contexto do **enlace local**.

Imagine:

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

Os quadros de enlace são utilizados em cada trecho.

De forma simplificada:

```text
TRECHO 1

PC ─────────► Roteador 1

MAC:
PC → Roteador 1
```

Depois:

```text
TRECHO 2

Roteador 1 ─────────► Roteador 2

MAC:
Roteador 1 → Roteador 2
```

Depois:

```text
TRECHO 3

Roteador 2 ─────────► Roteador 3

MAC:
Roteador 2 → Roteador 3
```

O endereço MAC do computador de origem não é simplesmente carregado como o endereço de enlace através de todos os roteadores até o servidor.

---

# 22. Exemplo completo

Imagine que seu computador possua:

```text
IP:
192.168.1.10

Máscara:
255.255.255.0

Gateway:
192.168.1.1

DNS:
192.168.1.1

MAC:
AA:BB:CC:DD:EE:FF
```

Cada informação possui uma função:

### IP

```text
192.168.1.10
```

> Este é o endereço IP do dispositivo nessa rede.

### Máscara

```text
255.255.255.0
```

> Define a divisão entre a parte da rede e a parte dos hosts.

### Gateway

```text
192.168.1.1
```

> É a saída utilizada para alcançar outras redes.

### DNS

```text
192.168.1.1
```

> É o servidor DNS configurado para resolver nomes de domínio.

### MAC

```text
AA:BB:CC:DD:EE:FF
```

> Identifica a interface de rede no contexto da comunicação de enlace.

---

# 23. Exemplo: acessando um site

Imagine que você digite:

```text
www.google.com
```

Uma visão simplificada do processo seria:

```text
1. Usuário digita o domínio
          ↓
2. DNS resolve o nome
          ↓
3. O dispositivo obtém o IP do destino
          ↓
4. A máscara ajuda a verificar se o destino é local
          ↓
5. Se estiver fora da rede local:
          ↓
6. O tráfego é enviado ao Gateway
          ↓
7. O roteador encaminha os pacotes
          ↓
8. Os pacotes atravessam outras redes
          ↓
9. O destino recebe os dados
```

No trecho local, os quadros utilizam endereços MAC.

---

# 24. Como tudo se relaciona

Podemos visualizar:

```text
                 DISPOSITIVO
                      │
        ┌─────────────┼─────────────┐
        │             │             │
       MAC            IP           DNS
        │             │             │
        │          Máscara          │
        │             │             │
        │          Gateway          │
        │             │             │
        └─────────────┼─────────────┘
                      ↓
                  REDE LOCAL
                      ↓
                   ROTEADOR
                      ↓
                   INTERNET
```

Essas informações não fazem a mesma coisa.

Elas trabalham juntas para permitir que os dispositivos se comuniquem.

---

# 25. Comparação rápida

| Conceito | Pergunta que ele ajuda a responder |
|---|---|
| **IP** | Qual é o endereço lógico desse dispositivo na rede? |
| **Máscara** | Qual parte do IP representa a rede e qual representa o host? |
| **Gateway** | Por onde saio da minha rede para chegar a outras redes? |
| **DNS** | Qual IP corresponde a este nome de domínio? |
| **MAC** | Qual interface de rede é o destino neste enlace local? |

---

# 26. Analogia

Podemos criar uma analogia simples com uma cidade.

### IP

É como o **endereço de uma casa**.

```text
Rua X, número 100
```

### Máscara

Ajuda a determinar a qual **rede/região** aquele endereço pertence.

### Gateway

É como uma **saída da região** para chegar a outras regiões.

### DNS

É como procurar:

```text
"Casa do João"
       ↓
Endereço da casa
```

### MAC

É uma identificação associada à **interface de comunicação** utilizada naquele trecho da rede.

---

# 27. Cuidado com a analogia

As analogias ajudam a entender, mas não devem ser levadas ao pé da letra.

Principalmente:

```text
IP ≠ endereço físico permanente
```

Um endereço IP pode mudar.

Por exemplo:

```text
Hoje:
192.168.1.10
```

Depois:

```text
192.168.1.15
```

Isso pode acontecer devido ao funcionamento do DHCP, entre outros fatores.

O MAC, por sua vez, está associado à interface de rede, embora dispositivos modernos possam utilizar mecanismos de **MAC privado/aleatório**, especialmente em redes Wi-Fi.

---

# 28. Resumo para memorizar

```text
IP
→ Endereço lógico do dispositivo

MÁSCARA
→ Define rede e host

GATEWAY
→ Saída para outras redes

DNS
→ Nome de domínio → IP

MAC
→ Identificação da interface no enlace
```

Uma forma ainda mais simples:

```text
IP
"Qual é meu endereço lógico?"

MÁSCARA
"Qual é minha rede?"

GATEWAY
"Por onde saio da minha rede?"

DNS
"Qual IP corresponde a esse nome?"

MAC
"Qual é a interface de rede neste enlace?"
```

---

# 29. Relação com as camadas de rede

Esses conceitos começam a se encaixar no modelo de comunicação:

```text
Aplicação
   ↓
HTTP / HTTPS
   ↓
TCP / UDP
   ↓
IP
   ↓
Ethernet / Wi-Fi
   ↓
MAC
   ↓
Meio físico
```

De forma simplificada:

```text
DNS
↓
descobre o endereço IP

IP
↓
permite o endereçamento e encaminhamento entre redes

MAC
↓
participa da entrega do quadro no enlace local
```

---

# 30. Relação com programação

Esses conceitos serão importantes posteriormente na programação.

Quando você começar a criar aplicações:

```text
Front-end
    ↓
HTTP/HTTPS
    ↓
API
    ↓
Back-end
    ↓
Banco de dados
```

toda essa comunicação dependerá da infraestrutura de rede estudada aqui.

Por exemplo:

```text
Java
 ↓
HTTP
 ↓
TCP
 ↓
IP
 ↓
Ethernet/Wi-Fi
 ↓
Roteador
 ↓
Internet
 ↓
Servidor
```

Por isso, entender redes antes de avançar para programação ajuda a compreender **o que realmente acontece quando uma aplicação se comunica com outra máquina**.

---

# 31. Conclusão

**IP, máscara, gateway, DNS e MAC são conceitos diferentes, mas trabalham juntos.**

```text
MAC
↓
Comunicação no enlace local

IP
↓
Endereçamento lógico e comunicação entre redes

Máscara
↓
Determina a rede e os hosts

Gateway
↓
Saída para outras redes

DNS
↓
Resolve nomes em endereços IP
```

> **Ideia principal:** um dispositivo precisa saber seu endereço IP, entender qual é sua rede através da máscara, saber para onde enviar tráfego destinado a outras redes através do gateway, utilizar DNS quando precisar transformar nomes em IPs e utilizar a interface de rede/MAC na comunicação de enlace local.
