# ⭐ Topologia em Estrela

## 📌 O que é?

Na **topologia em estrela**, todos os dispositivos da rede são conectados a um **dispositivo central**.

Esse dispositivo central pode ser, por exemplo:

- Switch
- Hub
- Em alguns cenários, um ponto central de comunicação

A estrutura lembra uma estrela:

```text
              PC1
               │
               │
PC2 ───────── SWITCH ───────── PC3
               │
               │
              PC4
```

O **switch fica no centro** e os dispositivos ficam conectados a ele.

---

# 🔌 Como funciona?

Imagine quatro computadores:

```text
PC1
 │
PC2 ─── SWITCH ─── PC3
 │
PC4
```

Na prática, cada computador possui sua própria conexão com o switch:

```text
PC1 ─────┐
PC2 ─────┤
PC3 ─────┼── SWITCH
PC4 ─────┘
```

Se o PC1 quiser se comunicar com o PC3:

```text
PC1
 │
 ↓
SWITCH
 │
 ↓
PC3
```

O computador não precisa estar conectado diretamente ao PC3.

O **switch recebe o quadro e encaminha para o destino apropriado**.

---

# 🧠 Por que o switch é importante?

O switch trabalha principalmente utilizando os **endereços MAC** dos dispositivos.

Por exemplo:

```text
PC1
MAC: AA:AA:AA:AA:AA:01

PC2
MAC: BB:BB:BB:BB:BB:02

PC3
MAC: CC:CC:CC:CC:CC:03
```

O switch aprende quais endereços MAC estão associados às suas portas.

Assim, quando recebe um quadro destinado ao PC3, pode encaminhá-lo para a porta onde o PC3 está conectado.

```text
PC1
 │
 │ quadro destinado ao MAC do PC3
 ↓
SWITCH
 │
 │
 ↓
PC3
```

---

# ✅ Vantagens da topologia estrela

## 1. Fácil de instalar

Cada dispositivo possui sua própria conexão com o equipamento central.

```text
PC1 ──┐
PC2 ──┤
PC3 ──┼── SWITCH
PC4 ──┘
```

Isso facilita a organização da rede.

---

## 2. Fácil de identificar problemas

Imagine que o cabo do PC3 apresente defeito:

```text
PC1 ──┐
PC2 ──┤
PC3 ──X── SWITCH
PC4 ──┘
```

Normalmente:

```text
PC1 → funciona
PC2 → funciona
PC3 → sem conexão
PC4 → funciona
```

O problema fica mais localizado.

---

## 3. Fácil adicionar dispositivos

É possível conectar outro computador ao switch:

```text
PC1 ──┐
PC2 ──┤
PC3 ──┼── SWITCH ─── PC5
PC4 ──┘
```

Desde que exista uma porta disponível e a infraestrutura permita.

---

# ❌ Desvantagem principal

O equipamento central é um **ponto crítico da rede**.

Se o switch parar de funcionar:

```text
PC1 ──┐
PC2 ──┤
PC3 ──X── SWITCH
PC4 ──┘
```

Os dispositivos conectados a ele podem perder a comunicação entre si.

Portanto:

> **Problema em um cabo individual → geralmente afeta apenas aquele dispositivo.**

> **Problema no equipamento central → pode afetar vários dispositivos.**

---

# 🔄 Estrela x Barramento

### Barramento

```text
========================
 │       │       │
PC1     PC2     PC3
```

Os dispositivos compartilham um meio principal.

### Estrela

```text
       PC1
        │
PC2 ─ SWITCH ─ PC3
        │
       PC4
```

Cada dispositivo possui uma conexão com o ponto central.

---

# 🌐 Estrela em redes modernas

Uma rede doméstica atual pode ser visualizada de forma semelhante:

```text
                Internet
                   │
                Roteador
                   │
              ┌────┴────┐
              │         │
           Wi-Fi     Ethernet
              │         │
           Notebook    Switch
                        │
                   ┌────┼────┐
                   │    │    │
                  PC   TV  Console
```

Aqui existem várias tecnologias e equipamentos trabalhando juntos.

Por isso, na prática, uma rede pode ter uma **combinação de estruturas**.

---

# ⚠️ Uma observação importante

Não confunda:

**Topologia estrela**

com

**rede Wi-Fi**.

Uma rede Wi-Fi também pode possuir uma organização semelhante a uma estrela:

```text
       Notebook
           \
            \
Celular ─── Access Point
            /
           /
       TV
```

O Access Point funciona como ponto central de comunicação sem fio.

Mas isso não significa que "estrela = Wi-Fi".

Topologia e meio/tecnologia de transmissão são conceitos diferentes.

---

# 🧠 O que guardar

A ideia principal é:

```text
              Dispositivo
                   │
                   │
Dispositivo ─── PONTO CENTRAL ─── Dispositivo
                   │
                   │
              Dispositivo
```

> **Topologia estrela = dispositivos conectados a um ponto central.**

Em redes Ethernet modernas, esse ponto central geralmente é um **switch**.

### E lembre:

```text
Cabo de um PC com problema
        ↓
normalmente afeta aquele PC

Switch central com problema
        ↓
pode afetar vários dispositivos
```
