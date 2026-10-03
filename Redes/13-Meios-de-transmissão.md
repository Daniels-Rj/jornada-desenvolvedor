# 📡 Meios de Transmissão

## 📌 O que são meios de transmissão?

**Meio de transmissão** é o caminho utilizado para transportar os dados de um dispositivo para outro.

Exemplo:

```text
Computador
    │
    │ dados
    ↓
Meio de transmissão
    │
    ↓
Outro dispositivo
```

Os meios de transmissão podem ser divididos principalmente em:

- **Meios guiados (com fio)**
- **Meios não guiados (sem fio)**

---

# 🔌 1. Meios Guiados

Nos meios guiados, o sinal percorre um **meio físico**, como um cabo.

Os principais exemplos são:

- Par trançado
- Cabo coaxial
- Fibra óptica

---

# 🟦 Par Trançado

É um dos meios mais utilizados em redes Ethernet.

O cabo possui pares de fios de cobre que são **trançados entre si**.

```text
~~~~~~
~~~~~~
~~~~~~
```

O trançamento ajuda a reduzir interferências eletromagnéticas.

## Exemplos

Categorias comuns:

- Cat5e
- Cat6
- Cat6a
- Cat7
- Cat8

O conector mais conhecido em redes Ethernet é o **RJ-45**.

Exemplo:

```text
PC ─────── cabo Ethernet ─────── Switch
```

---

# 🟫 Cabo Coaxial

Possui uma estrutura com:

```text
┌───────────────────────┐
│ Revestimento externo  │
│   ┌───────────────┐   │
│   │ Blindagem     │   │
│   │  ┌─────────┐  │   │
│   │  │Condutor │  │   │
│   │  └─────────┘  │   │
│   └───────────────┘   │
└───────────────────────┘
```

Possui um condutor central protegido por materiais isolantes e blindagem.

Foi muito utilizado em redes Ethernet antigas.

Também é utilizado em outras aplicações, como:

- TV a cabo
- Sistemas de antena
- CFTV
- Comunicação de radiofrequência

---

# 💡 Fibra Óptica

Na fibra óptica, os dados são transmitidos utilizando **luz**.

```text
Computador
    │
    ↓
[Transmissor]
    │
    │ luz
    ↓
══════════════════════════
      Fibra óptica
══════════════════════════
    │
    ↓
[Receptor]
    │
    ↓
Outro dispositivo
```

Em vez de transportar sinais elétricos pelo cobre, a fibra utiliza pulsos de luz.

## Vantagens

- Alta capacidade de transmissão
- Baixa atenuação em longas distâncias
- Não sofre interferência eletromagnética da mesma maneira que cabos metálicos
- Excelente para grandes distâncias

Por isso, a fibra é muito utilizada em:

- Backbones
- Data centers
- Redes de operadoras
- Cabos submarinos
- Internet de longa distância

---

# 📡 2. Meios Não Guiados

Nos meios não guiados, não existe um cabo físico conduzindo o sinal de uma ponta até a outra.

A transmissão ocorre através do espaço utilizando **ondas eletromagnéticas**.

Exemplos:

- Wi-Fi
- Bluetooth
- Rádio
- Comunicação via satélite
- Redes celulares

```text
      📡
       )))))))))
      ))))))))))) 
     )))))))))))))
           ↓
        📱
```

---

# 📶 Wi-Fi

O Wi-Fi utiliza ondas de rádio para transmitir dados.

Exemplo:

```text
Notebook
    ))) 
     )))
      ))) 
    Roteador
```

Não existe um cabo ligando fisicamente o notebook ao roteador.

---

# 🔵 Bluetooth

Também utiliza ondas de rádio.

É utilizado principalmente para comunicação de curta distância.

Exemplos:

- Fones de ouvido
- Teclados
- Mouses
- Controles
- Smartphones

---

# 🛰️ Satélite

A comunicação pode acontecer utilizando ondas de rádio entre uma estação terrestre e um satélite.

```text
Estação terrestre
       ↑
       │
       │ ondas de rádio
       ↓
    🛰️ Satélite
       ↑
       │
       ↓
Outra estação
```

É útil para comunicação em grandes áreas e locais onde outras infraestruturas são difíceis de instalar.

---

# 📊 Comparação

| Meio | Tipo | Sinal | Exemplo |
|---|---|---|---|
| Par trançado | Guiado | Elétrico | Ethernet |
| Coaxial | Guiado | Elétrico | TV a cabo |
| Fibra óptica | Guiado | Luz | Internet/backbone |
| Wi-Fi | Não guiado | Rádio | Rede sem fio |
| Bluetooth | Não guiado | Rádio | Fone sem fio |
| Satélite | Não guiado | Ondas de rádio | Comunicação via satélite |

---

# 🧠 Guiado x Não Guiado

Uma maneira fácil de lembrar:

```text
GUIADO
   ↓
Existe um meio físico guiando o sinal

Cabo de cobre
Fibra óptica
Cabo coaxial
```

```text
NÃO GUIADO
   ↓
O sinal se propaga pelo espaço

Wi-Fi
Bluetooth
Rádio
Satélite
```

---

# 🔗 Relação com o que você já estudou

Agora podemos juntar vários conceitos.

Imagine uma rede doméstica:

```text
                    INTERNET
                       │
                       │ fibra
                       ↓
                  ROTEADOR
                 /        \
                /          \
           Wi-Fi          Ethernet
             ↓                ↓
         Notebook            PC
```

Aqui temos **diferentes meios de transmissão na mesma rede**.

### Entre o provedor e sua casa

Pode existir:

```text
Fibra óptica
```

### Do roteador até o notebook

Pode existir:

```text
Wi-Fi
```

### Do roteador até o PC

Pode existir:

```text
Cabo Ethernet
```

Portanto:

> **Uma rede não precisa utilizar apenas um único meio de transmissão.**

---

# 🌊 Sinal x Meio de transmissão

É importante não confundir os dois.

### Meio

É **por onde** o sinal passa.

Exemplo:

```text
Fibra óptica
```

### Sinal

É **o que transporta a informação** através daquele meio.

Exemplo:

```text
Pulsos de luz
```

Outro exemplo:

```text
Meio: cabo de cobre
Sinal: sinal elétrico
```

E:

```text
Meio: espaço
Sinal: ondas eletromagnéticas
```

---

# 🌐 Exemplo: acessando um site

Quando você acessa um site, os dados podem passar por vários meios diferentes.

Uma representação simplificada:

```text
Seu computador
      │
      │ Wi-Fi
      ↓
   Roteador
      │
      │ fibra
      ↓
Operadora
      │
      │ fibra óptica
      ↓
Rede da Internet
      │
      ↓
Servidor
```

Ou seja, a informação pode atravessar **vários meios de transmissão diferentes durante o caminho**.

---

# 🧠 O que realmente guardar

Não precisa decorar todos os detalhes técnicos agora.

O principal é:

```text
MEIOS DE TRANSMISSÃO

        ┌── GUIADOS
        │
        ├── Par trançado
        ├── Coaxial
        └── Fibra óptica

        └── NÃO GUIADOS
            ├── Wi-Fi
            ├── Bluetooth
            ├── Rádio
            └── Satélite
```

### Frase para memorizar:

> **Meio de transmissão é o caminho utilizado para transportar os dados entre dispositivos.**

E lembre:

> **Cobre → sinal elétrico**

> **Fibra → luz**

> **Ar/espaço → ondas eletromagnéticas**
