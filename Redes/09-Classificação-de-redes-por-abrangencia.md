# Classificação de Redes por Abrangência

## 1. Introdução

As redes de computadores podem ser classificadas de diferentes maneiras.

Uma das classificações mais importantes é feita de acordo com a **abrangência**, ou seja:

> **Qual área geográfica a rede consegue cobrir?**

Quanto maior a área que uma rede precisa atender, maior tende a ser sua abrangência.

As principais classificações são:

- **PAN** — Personal Area Network
- **LAN** — Local Area Network
- **CAN** — Campus Area Network
- **MAN** — Metropolitan Area Network
- **WAN** — Wide Area Network
- **GAN** — Global Area Network

Uma forma de visualizar:

```text
PAN
 ↓
LAN
 ↓
CAN
 ↓
MAN
 ↓
WAN
 ↓
GAN
```

De forma geral, estamos aumentando a área de cobertura.

---

# 2. PAN — Personal Area Network

**PAN** significa:

> **Personal Area Network**

Em português:

> **Rede de Área Pessoal**

É uma rede utilizada para conectar dispositivos próximos a uma pessoa.

Exemplo:

```text
        Smartphone
          /    \
         /      \
        ↓        ↓
   Smartwatch   Fone Bluetooth
```

Também podemos ter:

```text
Notebook
   ↕
Smartphone
   ↕
Fone Bluetooth
```

---

# 3. Tecnologias utilizadas em PAN

Uma PAN pode utilizar tecnologias como:

- Bluetooth;
- USB;
- NFC;
- Outras tecnologias de curto alcance.

Um exemplo muito comum é o Bluetooth.

```text
Smartphone
     │
     │ Bluetooth
     ↓
Fone de ouvido
```

Os dispositivos estão próximos uns dos outros.

---

# 4. Exemplo de PAN no dia a dia

Imagine uma pessoa utilizando:

```text
        Smartphone
       /     |     \
      ↓      ↓      ↓
 Relógio   Fone   Notebook
```

Todos esses dispositivos podem estar conectados ou interagindo próximos ao usuário.

Isso é um exemplo de uma **PAN**.

---

# 5. LAN — Local Area Network

**LAN** significa:

> **Local Area Network**

Em português:

> **Rede de Área Local**

É uma rede que cobre uma área geográfica relativamente pequena.

Exemplos:

- Casa;
- Escritório;
- Laboratório;
- Sala;
- Pequena empresa;
- Escola.

Exemplo de uma rede doméstica:

```text
              ROTEADOR
             /   |   \
            /    |    \
           ↓     ↓     ↓
        Notebook PC   Smartphone
```

Esses dispositivos podem estar conectados à mesma rede local.

---

# 6. Tecnologias utilizadas em LAN

Uma LAN pode utilizar:

### Ethernet

```text
Computador
    │
    │ cabo de rede
    ↓
  Switch
```

### Wi-Fi

```text
Smartphone
     )))
      )))
       ↓
    Roteador
```

Portanto:

> **LAN não significa necessariamente rede cabeada.**

Uma LAN pode ser:

- Cabeada;
- Sem fio;
- Ou uma combinação das duas.

---

# 7. Exemplo de LAN residencial

Imagine sua casa:

```text
                    ROTEADOR
                  /    |     \
                 /     |      \
                ↓      ↓       ↓
             Notebook  PC   Smartphone
```

Todos esses dispositivos podem fazer parte da mesma **LAN**.

A rede local pode utilizar:

```text
Wi-Fi
Ethernet
IP
DHCP
DNS
```

---

# 8. CAN — Campus Area Network

**CAN** significa:

> **Campus Area Network**

Em português:

> **Rede de Área de Campus**

É utilizada para conectar várias redes locais dentro de uma área maior, como:

- Universidades;
- Complexos empresariais;
- Campi;
- Grandes instituições.

Exemplo:

```text
          CAMPUS
             │
      ┌──────┼──────┐
      ↓      ↓      ↓
   Prédio A Prédio B Prédio C
      │      │      │
     LAN    LAN    LAN
```

As várias LANs podem ser interligadas formando uma rede maior.

---

# 9. Exemplo de CAN

Imagine uma universidade.

Ela possui:

```text
Prédio de Engenharia
       ↓
      LAN

Prédio de Administração
       ↓
      LAN

Biblioteca
       ↓
      LAN

Laboratórios
       ↓
      LAN
```

Essas redes podem ser interligadas:

```text
              CAMPUS
                 │
       ┌─────────┼─────────┐
       ↓         ↓         ↓
     LAN A     LAN B      LAN C
       │         │         │
    Prédio A  Prédio B  Biblioteca
```

Isso caracteriza uma **CAN**.

---

# 10. MAN — Metropolitan Area Network

**MAN** significa:

> **Metropolitan Area Network**

Em português:

> **Rede de Área Metropolitana**

É uma rede que cobre uma área maior que uma LAN ou CAN, podendo abranger uma cidade ou região metropolitana.

Exemplo conceitual:

```text
              CIDADE
   ┌───────────┼───────────┐
   ↓           ↓           ↓
Empresa A   Empresa B   Empresa C
   │           │           │
   └───────────┼───────────┘
               ↓
              MAN
```

---

# 11. Exemplo de MAN

Imagine uma organização que possui vários prédios espalhados por uma cidade.

```text
          Prédio A
             │
             │
             ▼
          ┌─────┐
          │ MAN │
          └─────┘
           /   \
          /     \
         ↓       ↓
    Prédio B   Prédio C
```

As diferentes redes locais podem ser conectadas através de uma infraestrutura metropolitana.

---

# 12. WAN — Wide Area Network

**WAN** significa:

> **Wide Area Network**

Em português:

> **Rede de Área Ampla**

É uma rede que cobre uma área geográfica muito grande.

Pode conectar:

- Cidades;
- Estados;
- Países;
- Continentes.

Exemplo:

```text
Rio de Janeiro
       │
       │
       ▼
     WAN
       │
       ▼
São Paulo
       │
       ▼
Brasília
```

---

# 13. Exemplo de WAN de uma empresa

Uma empresa pode possuir escritórios em diferentes cidades:

```text
              MATRIZ
           Rio de Janeiro
                 │
                 │
                WAN
                 │
        ┌────────┴────────┐
        ↓                 ↓
    São Paulo          Brasília
```

Cada escritório pode possuir sua própria LAN.

```text
LAN
 ↓
Escritório RJ
```

```text
LAN
 ↓
Escritório SP
```

```text
LAN
 ↓
Escritório Brasília
```

A WAN conecta essas redes.

---

# 14. Internet e WAN

A Internet possui características de uma rede de abrangência global e é formada pela interligação de inúmeras redes.

Podemos visualizar de maneira simplificada:

```text
LAN
 │
 ↓
WAN
 │
 ↓
Outras redes
 │
 ↓
Internet
```

Mas é importante não dizer simplesmente:

> "Internet = uma WAN."

A Internet é uma **rede de redes**, formada por diversas redes independentes e interconectadas.

---

# 15. GAN — Global Area Network

**GAN** significa:

> **Global Area Network**

Em português:

> **Rede de Área Global**

Representa redes com alcance global.

Podemos pensar em:

```text
País
 ↓
Continente
 ↓
Mundo
```

Uma rede global pode interligar estruturas distribuídas em diferentes países e continentes.

---

# 16. Comparação das classificações

| Tipo | Nome | Abrangência aproximada | Exemplo |
|---|---|---|---|
| **PAN** | Personal Area Network | Ao redor de uma pessoa | Bluetooth |
| **LAN** | Local Area Network | Casa, sala, escritório | Rede doméstica |
| **CAN** | Campus Area Network | Campus/complexo | Universidade |
| **MAN** | Metropolitan Area Network | Cidade/região metropolitana | Rede metropolitana |
| **WAN** | Wide Area Network | Grandes regiões/países/continentes | Rede corporativa entre cidades |
| **GAN** | Global Area Network | Global | Rede mundial |

---

# 17. Visualização da abrangência

Uma forma de memorizar:

```text
              GAN
       ┌───────────────┐
       │     GLOBAL    │
       │               │
       │     WAN       │
       │   ┌───────┐   │
       │   │   MAN │   │
       │   │ ┌───┐ │   │
       │   │ │CAN│ │   │
       │   │ │┌─┐│ │   │
       │   │ ││LAN│ │  │
       │   │ │└─┘│ │   │
       │   │ └───┘ │   │
       │   └───────┘   │
       └───────────────┘
```

E uma sequência mais simples:

```text
PAN
 ↓
LAN
 ↓
CAN
 ↓
MAN
 ↓
WAN
 ↓
GAN
```

---

# 18. PAN x LAN

Essa diferença é bastante importante.

### PAN

Foco em dispositivos próximos a uma pessoa.

```text
        Pessoa
          │
     ┌────┼────┐
     ↓    ↓    ↓
   Fone  Celular Relógio
```

### LAN

Foco em uma área local.

```text
             Roteador
          /      |      \
         ↓       ↓       ↓
       PC      Notebook  Celular
```

---

# 19. LAN x CAN

### LAN

Normalmente cobre uma área local:

```text
Casa
 ↓
LAN
```

### CAN

Pode conectar várias LANs dentro de uma área maior:

```text
      CAMPUS
         │
   ┌─────┼─────┐
   ↓     ↓     ↓
 LAN   LAN    LAN
```

---

# 20. CAN x MAN

### CAN

Normalmente está relacionada a um campus ou complexo específico.

```text
Universidade
     ↓
   CAN
```

### MAN

Pode abranger uma área metropolitana/cidade.

```text
Cidade
  ↓
 MAN
```

---

# 21. MAN x WAN

### MAN

Abrangência metropolitana.

```text
Cidade
  ↓
 MAN
```

### WAN

Abrangência muito maior.

```text
Cidade
  ↓
Estado
  ↓
País
  ↓
WAN
```

---

# 22. PAN não significa necessariamente Internet

Um exemplo:

```text
Celular
   )))
    ))) Bluetooth
     ↓
Fone
```

Você possui uma comunicação entre dispositivos, mas isso não significa que o fone esteja conectado à Internet.

Portanto:

> **Uma rede pode existir sem necessariamente possuir acesso à Internet.**

---

# 23. LAN também não significa Internet

Imagine dois computadores conectados diretamente:

```text
PC A
  │
  │ Ethernet
  │
PC B
```

Eles podem formar uma pequena rede local mesmo sem acesso à Internet.

Podem, por exemplo, compartilhar arquivos.

```text
PC A ←──────→ PC B
```

A Internet é uma possibilidade de conexão externa, não uma exigência para existir uma LAN.

---

# 24. Internet x abrangência

É comum pensar:

```text
Internet
=
maior tipo de rede
```

Mas precisamos ter cuidado.

A Internet não é simplesmente uma rede única classificada apenas pelo tamanho.

Ela é:

> **Uma rede mundial formada pela interconexão de inúmeras redes.**

Podemos visualizar:

```text
LAN
 │
 ↓
Provedor
 │
 ↓
Outras redes
 │
 ↓
Backbones
 │
 ↓
Outras redes
 │
 ↓
Servidores
```

---

# 25. Relação com o que já estudamos

Esse assunto conecta vários conceitos anteriores.

Já estudamos:

```text
Computadores
      ↓
Redes
      ↓
Ponto a Ponto / Cliente-Servidor
      ↓
Servidores
      ↓
Classificação por abrangência
```

Agora conseguimos visualizar uma rede de uma empresa:

```text
                   WAN
                    │
        ┌───────────┴───────────┐
        ↓                       ↓
     Escritório              Escritório
        │                       │
       LAN                     LAN
        │                       │
     PCs/Server              PCs/Server
```

---

# 26. Relação com Internet

Uma rede doméstica pode ser uma LAN:

```text
          ROTEADOR
         /   |   \
        ↓    ↓    ↓
       PC   TV  Celular
```

Essa LAN pode se conectar ao provedor:

```text
LAN
 ↓
Roteador
 ↓
Provedor
 ↓
Internet
```

A partir daí, ela pode acessar servidores localizados em outras redes.

```text
Sua LAN
   ↓
Provedor
   ↓
Internet
   ↓
Servidor
```

---

# 27. Exemplo completo

Imagine uma empresa internacional:

```text
                    INTERNET / WAN
                         │
        ┌────────────────┼────────────────┐
        ↓                ↓                ↓
      BRASIL           EUA             PORTUGAL
        │                │                │
       LAN              LAN              LAN
        │                │                │
      PCs              PCs              PCs
        │                │                │
     Servidor        Servidor         Servidor
```

Dentro de cada local existem redes menores.

Essas redes podem estar conectadas através de redes de maior abrangência.

---

# 28. Uma observação importante

As classificações por abrangência são **conceitos de organização e alcance**, e não regras matemáticas rígidas.

Por exemplo, não existe uma única distância universal que determine:

```text
"até X metros é LAN"
"acima de X metros é MAN"
```

A classificação depende também do contexto, da infraestrutura e da forma como a rede é organizada.

---

# 29. O que preciso memorizar?

O mais importante é entender a ideia de **abrangência**.

```text
PAN
↓
Pessoa / dispositivos próximos

LAN
↓
Local / casa / escritório

CAN
↓
Campus / complexo

MAN
↓
Cidade / região metropolitana

WAN
↓
Grandes áreas / países / continentes

GAN
↓
Global
```

Uma maneira fácil de lembrar:

```text
P → Personal
L → Local
C → Campus
M → Metropolitan
W → Wide
G → Global
```

---

# 30. Resumo final

As redes podem ser classificadas de acordo com sua abrangência geográfica.

### PAN

```text
Área pessoal
```

Exemplo:

```text
Celular ↔ Fone Bluetooth
```

### LAN

```text
Área local
```

Exemplo:

```text
Rede de uma casa ou escritório
```

### CAN

```text
Área de campus
```

Exemplo:

```text
Rede de uma universidade
```

### MAN

```text
Área metropolitana
```

Exemplo:

```text
Rede abrangendo uma cidade
```

### WAN

```text
Área ampla
```

Exemplo:

```text
Rede conectando escritórios em diferentes cidades
```

### GAN

```text
Área global
```

Exemplo:

```text
Rede com alcance mundial
```

---

# 31. Mapa mental

```text
                 CLASSIFICAÇÃO POR ABRANGÊNCIA
                              │
          ┌───────────────────┼───────────────────┐
          │                   │                   │
         PAN                 LAN                 CAN
          │                   │                   │
       Pessoa               Local              Campus
          │                   │                   │
      Bluetooth          Casa/Empresa        Universidade
                              │
                              ↓
                             MAN
                              │
                            Cidade
                              │
                              ↓
                             WAN
                              │
                    Países/Continentes
                              │
                              ↓
                             GAN
                              │
                            Global
```

> **Ideia principal:** a classificação por abrangência indica principalmente o tamanho/alcance geográfico da rede, indo de uma rede pessoal (PAN) até redes de alcance global (GAN).
