# 🌐 História da Internet e da World Wide Web

A Internet e a Web não foram criadas por uma única pessoa. Elas surgiram através de várias pesquisas, tecnologias e pessoas ao longo de décadas.

---

## 📡 1. Antes da Internet

Antes dos computadores estarem conectados em rede, já existiam tecnologias para transmitir informações à distância.

### Samuel Morse

No século XIX, **Samuel Morse** desenvolveu um sistema de telégrafo elétrico e o **Código Morse**.

O telégrafo permitia transmitir mensagens através de fios usando sinais elétricos.

### Alexander Graham Bell

Em 1876, **Alexander Graham Bell** recebeu uma famosa patente relacionada ao telefone.

O telefone permitiu transmitir **voz através de uma rede de comunicação**.

Essas tecnologias ajudaram a estabelecer uma ideia importante:

> A informação poderia ser transmitida à distância sem transportar fisicamente a mensagem.

---

## 💻 2. A ideia de conectar computadores

Durante a década de 1960, pesquisadores começaram a pensar em uma rede que pudesse conectar computadores e permitir o compartilhamento de informações e recursos.

### J.C.R. Licklider

**J.C.R. Licklider** foi um dos pesquisadores que imaginou uma espécie de rede mundial de computadores.

Ele trabalhou com ideias que posteriormente ajudariam a influenciar o desenvolvimento das redes de computadores.

---

## 📦 3. Comutação de Pacotes

Um dos conceitos fundamentais para a Internet foi a **comutação de pacotes (Packet Switching)**.

A ideia é dividir uma mensagem em pequenos pedaços chamados **pacotes**.

Exemplo:

```text
Mensagem
   ↓
┌─────┬─────┬─────┬─────┐
│ P1  │ P2  │ P3  │ P4  │
└─────┴─────┴─────┴─────┘
```

Esses pacotes podem viajar pela rede e posteriormente ser reunidos para reconstruir a mensagem original.

### Paul Baran

**Paul Baran** pesquisou redes distribuídas e formas de comunicação capazes de continuar funcionando mesmo quando partes da rede apresentassem falhas.

### Donald Davies

**Donald Davies**, no Reino Unido, também desenvolveu de forma independente ideias fundamentais relacionadas à **comutação de pacotes**.

### Leonard Kleinrock

**Leonard Kleinrock** desenvolveu trabalhos teóricos importantes sobre redes de comunicação e filas, contribuindo para os fundamentos matemáticos das redes de pacotes.

---

## 🔬 4. ARPANET — 1969

Na década de 1960, a **ARPA (Advanced Research Projects Agency)**, ligada ao governo dos Estados Unidos, financiou pesquisas para conectar computadores de instituições de pesquisa.

O resultado foi a **ARPANET**.

Em **1969**, a ARPANET começou a operar conectando inicialmente quatro pontos:

- UCLA
- Stanford Research Institute
- UC Santa Barbara
- University of Utah

A ARPANET é considerada uma das principais precursoras da Internet moderna.

### Larry Roberts

**Larry Roberts** foi uma figura importante na organização e desenvolvimento do projeto ARPANET.

---

## 🌎 5. TCP/IP — A base da Internet moderna

À medida que diferentes redes começaram a surgir, apareceu um problema:

> Como fazer redes diferentes conseguirem conversar entre si?

A solução envolveu o desenvolvimento de protocolos de comunicação.

### Vint Cerf e Robert Kahn

**Vint Cerf** e **Robert Kahn** foram fundamentais no desenvolvimento do **TCP/IP**.

### TCP

**TCP — Transmission Control Protocol**

O TCP fornece mecanismos que permitem uma comunicação confiável entre dispositivos, incluindo controle da transmissão e reorganização dos dados recebidos.

### IP

**IP — Internet Protocol**

O IP é responsável pelo endereçamento e encaminhamento dos pacotes entre redes.

De forma simplificada:

```text
IP
↓
"Para onde esse pacote deve ir?"

TCP
↓
"Como controlar e organizar a comunicação?"
```

---

## 🌐 6. Internet

Uma característica fundamental da Internet é que ela não é simplesmente uma única rede.

Ela é uma:

> **Rede de redes.**

Diversas redes diferentes conseguem se comunicar utilizando protocolos comuns, principalmente a família **TCP/IP**.

### 1983 — Adoção do TCP/IP

Em **1º de janeiro de 1983**, a ARPANET passou oficialmente a utilizar TCP/IP.

Essa data é frequentemente considerada um marco importante no desenvolvimento da Internet moderna.

---

## 📖 7. DNS — Domain Name System

Conforme a Internet cresceu, surgiu outro problema:

> Os usuários não poderiam precisar memorizar endereços IP numéricos para acessar cada serviço.

Por exemplo:

```text
142.250.xxx.xxx
```

seria muito mais difícil de memorizar do que:

```text
google.com
```

### Paul Mockapetris

**Paul Mockapetris** criou o **DNS (Domain Name System)**.

O DNS permite associar nomes de domínio a endereços IP.

De forma simplificada:

```text
google.com
     ↓
    DNS
     ↓
Endereço IP
     ↓
Servidor
```

---

## 🌍 8. World Wide Web

Agora chegamos a uma das partes mais importantes da história.

### Tim Berners-Lee

Em **1989**, enquanto trabalhava no **CERN**, o físico e cientista da computação britânico **Tim Berners-Lee** propôs um sistema para facilitar o compartilhamento e a conexão de informações entre pesquisadores.

Esse sistema se tornou a:

# World Wide Web — WWW

---

## 🧩 O que Tim Berners-Lee criou?

Berners-Lee desenvolveu componentes fundamentais da Web:

### HTML

**HTML — HyperText Markup Language**

É utilizado para estruturar documentos e páginas da Web.

Exemplo:

```html
<h1>Minha página</h1>
<p>Olá, mundo!</p>
```

### HTTP

**HTTP — HyperText Transfer Protocol**

É um protocolo utilizado para comunicação entre clientes, como navegadores, e servidores Web.

De maneira simplificada:

```text
Navegador
    ↓
   HTTP
    ↓
Servidor
    ↓
Resposta
    ↓
Navegador
```

### URL

**URL — Uniform Resource Locator**

É utilizada para identificar e localizar recursos na Web.

Exemplo:

```text
https://www.exemplo.com/pagina
```

### Primeiro navegador Web

Berners-Lee também criou o primeiro navegador/editor da Web, chamado originalmente de:

```text
WorldWideWeb
```

### Primeiro servidor Web

Ele também criou o primeiro servidor Web, utilizando um computador **NeXT** no CERN.

### Primeiro site Web

O primeiro site da Web foi:

```text
http://info.cern.ch
```

---

## ⚠️ 9. Internet ≠ World Wide Web

Essa é uma das coisas mais importantes para entender.

**Tim Berners-Lee não criou a Internet.**

A Internet já estava sendo desenvolvida através de redes como a ARPANET e de protocolos como TCP/IP.

Berners-Lee criou a **World Wide Web**, que funciona **sobre a Internet**.

Podemos visualizar assim:

```text
┌─────────────────────────────────────┐
│              INTERNET               │
│                                     │
│  Cabos                              │
│  Fibra óptica                       │
│  Wi-Fi                              │
│  Roteadores                         │
│  TCP/IP                             │
│  Redes de computadores              │
│                                     │
│       ┌───────────────────┐         │
│       │       WEB         │         │
│       │                   │         │
│       │ HTML              │         │
│       │ HTTP              │         │
│       │ URLs              │         │
│       │ Sites             │         │
│       └───────────────────┘         │
│                                     │
└─────────────────────────────────────┘
```

### Analogia

Podemos imaginar a Internet como uma **rede de estradas**.

A Web seria um dos sistemas que utiliza essas estradas para transportar e acessar informações.

- **Internet** → infraestrutura de comunicação.
- **Web** → sistema que utiliza essa infraestrutura para disponibilizar páginas e recursos interligados.

---

## 🧠 10. Linha do tempo simplificada

```text
Século XIX
    ↓
Telégrafo — Samuel Morse
    ↓
Telefone — Bell e outros pioneiros
    ↓
Década de 1960
    ↓
Pesquisas sobre redes de computadores
    ↓
Comutação de pacotes
    ↓
1969
    ↓
ARPANET
    ↓
Década de 1970
    ↓
TCP/IP — Vint Cerf e Robert Kahn
    ↓
1983
    ↓
ARPANET adota TCP/IP
    ↓
1983
    ↓
DNS — Paul Mockapetris
    ↓
1989
    ↓
Tim Berners-Lee propõe a Web
    ↓
1990
    ↓
Primeiros componentes da Web
    ↓
World Wide Web
    ↓
Expansão da Internet e da Web
    ↓
Web moderna
```

---

## 👨‍💻 11. Pessoas importantes

| Pessoa | Contribuição |
|---|---|
| **Samuel Morse** | Telégrafo e Código Morse |
| **Alexander Graham Bell** | Desenvolvimento do telefone |
| **J.C.R. Licklider** | Ideias sobre redes globais de computadores |
| **Paul Baran** | Pesquisas sobre redes distribuídas e pacotes |
| **Donald Davies** | Comutação de pacotes |
| **Leonard Kleinrock** | Fundamentos teóricos das redes de pacotes |
| **Larry Roberts** | Desenvolvimento da ARPANET |
| **Vint Cerf** | TCP/IP |
| **Robert Kahn** | TCP/IP |
| **Paul Mockapetris** | DNS |
| **Tim Berners-Lee** | World Wide Web |

---

## 🔑 12. Conceitos importantes

- **ARPANET** → uma das principais precursoras da Internet.
- **Comutação de pacotes** → divide os dados em pequenos pacotes para transmissão.
- **TCP/IP** → conjunto fundamental de protocolos da Internet.
- **IP** → responsável pelo endereçamento e encaminhamento de pacotes.
- **TCP** → fornece mecanismos para comunicação confiável.
- **DNS** → associa nomes de domínio a endereços IP.
- **Internet** → rede mundial formada pela interconexão de diversas redes.
- **Web** → sistema de páginas e recursos interligados que funciona sobre a Internet.
- **HTML** → estrutura documentos da Web.
- **HTTP** → protocolo utilizado na comunicação da Web.
- **URL** → identifica e localiza recursos na Web.

---

## 🎯 13. Resumo Final

A história da Internet e da Web não pode ser atribuída a uma única pessoa.

Podemos resumir a evolução da seguinte maneira:

```text
Telecomunicações
       ↓
Redes de computadores
       ↓
Comutação de pacotes
       ↓
ARPANET
       ↓
TCP/IP
       ↓
Internet
       ↓
DNS
       ↓
World Wide Web
```

A **Internet** criou a infraestrutura para computadores e redes se comunicarem.

Depois, **Tim Berners-Lee criou a World Wide Web**, tornando muito mais simples acessar e conectar informações através de páginas, links e navegadores.

> **Internet é a infraestrutura de comunicação.**
>
> **Web é um sistema que utiliza essa infraestrutura.**
