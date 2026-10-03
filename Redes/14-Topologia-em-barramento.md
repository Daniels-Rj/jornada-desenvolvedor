# 🚌 Topologia em Barramento (Bus)

## 📌 O que é?

Na **topologia em barramento**, todos os dispositivos da rede são conectados a um **único meio de transmissão principal**, chamado de **barramento**.

Uma representação simplificada:

```text
====================================
     │          │          │
    PC1        PC2        PC3
```

O cabo principal funciona como um caminho compartilhado pelos dispositivos.

---

## 🔄 Como funciona?

Imagine que o PC1 queira enviar dados para o PC3:

```text
PC1
 │
 ↓
====================================
                  ↓
                 PC3
```

Os dados são colocados no meio de transmissão compartilhado.

Os dispositivos conectados ao barramento podem receber o sinal, mas o dispositivo destinado aos dados é quem deve processá-los.

---

# 🔌 Cabo principal

Uma característica importante dessa topologia é a existência de um **cabo principal compartilhado**.

Esse cabo pode ser chamado de:

- Barramento
- Backbone da topologia
- Meio compartilhado

Em implementações antigas de Ethernet, era comum utilizar **cabo coaxial**.

---

# ⚠️ Terminadores

Nas redes em barramento tradicionais, as extremidades do cabo principal precisavam ser terminadas corretamente.

```text
[TERMINADOR]
     │
====================================
     │       │       │
    PC1     PC2     PC3
====================================
                              │
                       [TERMINADOR]
```

Os terminadores ajudavam a evitar que o sinal elétrico sofresse reflexões nas extremidades do cabo.

---

# ✅ Vantagens

## 1. Estrutura simples

A rede possui uma estrutura relativamente simples:

```text
=============================
 │       │       │       │
PC1     PC2     PC3     PC4
```

---

## 2. Menor quantidade de cabos

Como os dispositivos compartilham um meio principal, não é necessário utilizar um cabo individual indo até um switch central como na topologia estrela.

---

## 3. Baixo custo em implementações antigas

A menor quantidade de infraestrutura podia tornar esse modelo mais barato em determinados cenários.

---

# ❌ Desvantagens

## 1. Falha no barramento

Essa é uma das principais desvantagens.

Se o cabo principal apresentar uma falha:

```text
====================X============
```

uma grande parte ou até toda a comunicação da rede pode ser interrompida.

---

## 2. Meio compartilhado

Todos os dispositivos utilizam o mesmo meio de transmissão.

Isso significa que existe uma maior necessidade de controlar o acesso ao meio.

Quando vários dispositivos tentam transmitir, pode haver **colisões** em determinadas tecnologias.

---

## 3. Desempenho

À medida que mais dispositivos utilizam o mesmo meio compartilhado, o desempenho pode ser prejudicado.

```text
Poucos dispositivos
      ↓
menos competição pelo meio

Muitos dispositivos
      ↓
mais competição pelo meio
```

---

## 4. Diagnóstico de problemas

Encontrar exatamente onde está um problema no cabo principal pode ser mais difícil.

---

# ⭐ Barramento x Estrela

## Barramento

```text
====================================
    │        │        │        │
   PC1      PC2      PC3      PC4
```

Todos compartilham o meio principal.

## Estrela

```text
          PC1
           │
PC2 ─── SWITCH ─── PC3
           │
          PC4
```

Cada dispositivo possui uma conexão com o ponto central.

---

# 🧠 Uma comparação simples

Imagine uma estrada.

### Barramento

Uma única estrada compartilhada:

```text
🚗 ─────────────── 🚗 ─────────────── 🚗
```

Todos utilizam o mesmo caminho.

### Estrela

Cada dispositivo possui uma ligação com um ponto central:

```text
          🚗
           \
            \
🚗 ─────── 🏢 ─────── 🚗
            /
           /
          🚗
```

O 🏢 representa o ponto central.

---

# 🏠 E a minha casa?

A rede doméstica que você descreveu anteriormente **não é uma topologia em barramento tradicional**.

Sua rede provavelmente se aproxima muito mais de:

```text
              ROTEADOR
             /   |   \
            /    |    \
          PC    TV   CELULAR
```

Ou seja, uma estrutura em **estrela**.

---

# ⚠️ Importante: barramento não significa "Internet"

O termo **barramento** aqui significa a forma como os dispositivos estão conectados.

Não significa:

> "um cabo que leva Internet para vários computadores".

É uma característica da **topologia da rede**.

---

# 🧠 O que guardar

A ideia principal é:

> **Topologia em barramento = vários dispositivos compartilhando um meio de transmissão principal.**

Memorize:

```text
🚌 BARRAMENTO
        ↓
MEIO PRINCIPAL COMPARTILHADO
        ↓
 VÁRIOS DISPOSITIVOS
```

E compare:

```text
🚌 Barramento → meio principal compartilhado

⭐ Estrela → ponto central

🕸️ Malha → vários caminhos

🔄 Anel → circuito fechado
```
