# Topologia de Redes

## 📌 O que é topologia de rede?

**Topologia de rede** é a forma como os dispositivos de uma rede estão organizados e conectados entre si.

Ela descreve principalmente **como os dispositivos se comunicam e como estão interligados**.

Os dispositivos podem ser:

- Computadores
- Servidores
- Roteadores
- Switches
- Impressoras
- Access Points
- Outros dispositivos de rede

> **Topologia = organização da rede.**

---

# 🔹 Principais tipos de topologia

As principais topologias estudadas são:

1. Barramento (Bus)
2. Estrela (Star)
3. Anel (Ring)
4. Malha (Mesh)
5. Árvore (Tree)
6. Híbrida (Hybrid)

---

# 🚌 1. Topologia em Barramento

Todos os dispositivos compartilham um **único meio de transmissão principal**.

```text
PC1 ─── PC2 ─── PC3 ─── PC4
          │
      Barramento
```

Uma representação mais tradicional:

```text
================================
     │       │       │
    PC1     PC2     PC3
```

## Características

- Todos os dispositivos utilizam o mesmo meio.
- Era comum em redes Ethernet antigas.
- Utilizava cabo coaxial em muitas implementações.

## Vantagens

- Estrutura simples.
- Utiliza menos cabos.
- Pode ter custo menor em pequenas instalações.

## Desvantagens

- Se o cabo principal apresentar problema, toda a rede pode ser afetada.
- O desempenho pode diminuir com muitos dispositivos.
- Diagnosticar problemas pode ser mais difícil.

Hoje é uma topologia muito menos comum em redes locais modernas.

---

# ⭐ 2. Topologia em Estrela

Os dispositivos são conectados a um **ponto central**.

Normalmente esse ponto central é um **switch**.

```text
             PC1
              │
              │
PC2 ─────── SWITCH ─────── PC3
              │
              │
             PC4
```

Essa é uma das formas mais comuns de organização de redes Ethernet modernas.

## Vantagens

- Fácil de instalar.
- Fácil de identificar problemas.
- Se um cabo de um computador apresentar problema, normalmente apenas aquele dispositivo perde a conexão.
- Fácil adicionar novos dispositivos.

## Desvantagem

O equipamento central é um ponto importante da rede.

Se o switch central parar de funcionar:

```text
PC1 ──┐
PC2 ──┤
PC3 ──┼── ❌ SWITCH
PC4 ──┘
```

os dispositivos conectados a ele podem perder comunicação entre si.

---

# 🔄 3. Topologia em Anel

Os dispositivos são conectados formando um **circuito fechado**.

```text
       PC1
      /   \
    PC2   PC4
      \   /
       PC3
```

Cada dispositivo possui conexão com os dispositivos vizinhos.

## Características

Os dados podem circular pelo anel seguindo uma determinada direção ou, dependendo da tecnologia, por caminhos diferentes.

## Vantagens

- Organização previsível da comunicação.
- Pode oferecer caminhos alternativos em algumas implementações.

## Desvantagens

- Uma falha pode afetar a comunicação dependendo de como o anel foi implementado.
- É menos comum em redes locais modernas.

---

# 🕸️ 4. Topologia em Malha (Mesh)

Na topologia em malha, existem **múltiplas conexões entre os dispositivos**.

### Malha completa

Cada dispositivo possui conexão direta com todos os outros.

```text
      PC1
     / | \
    /  |  \
  PC2--|--PC3
    \  |  /
     \ | /
      PC4
```

Quanto maior a quantidade de dispositivos, maior pode ser a quantidade de conexões necessárias.

## Principal característica

A grande vantagem é a **redundância**.

Se um caminho falhar, pode existir outro caminho disponível.

Isso é muito importante em redes que precisam de alta disponibilidade.

## Desvantagem

Pode ser:

- Mais cara
- Mais complexa
- Mais difícil de administrar

---

# 🌳 5. Topologia em Árvore

É uma estrutura hierárquica que pode ser vista como uma combinação de várias redes em estrela.

```text
             Roteador
                │
             Switch
           /       \
       Switch     Switch
       /   \       /   \
     PC1   PC2   PC3   PC4
```

É muito utilizada para representar redes maiores e hierárquicas.

Por exemplo:

```text
Empresa
   │
   ├── Setor Administrativo
   │      ├── PC
   │      └── PC
   │
   ├── RH
   │      ├── PC
   │      └── PC
   │
   └── TI
          ├── PC
          └── Servidor
```

---

# 🔀 6. Topologia Híbrida

É a combinação de **duas ou mais topologias diferentes**.

Por exemplo:

```text
      Estrela
         │
      Switch
      /    \
     /      \
 Estrela    Estrela
```

Uma empresa pode utilizar diferentes estruturas em diferentes partes da rede.

---

# 📊 Comparação

| Topologia | Organização | Principal característica |
|---|---|---|
| 🚌 Barramento | Linha principal | Meio compartilhado |
| ⭐ Estrela | Ponto central | Fácil gerenciamento |
| 🔄 Anel | Círculo | Dispositivos conectados em sequência |
| 🕸️ Malha | Vários caminhos | Redundância |
| 🌳 Árvore | Hierárquica | Organização em níveis |
| 🔀 Híbrida | Combinação | Mistura de topologias |

---

# ⚠️ Topologia física x lógica

Esse é um detalhe importante.

## Topologia física

Representa **como os dispositivos e cabos estão fisicamente conectados**.

Exemplo:

```text
PC1 ──┐
PC2 ──┼── SWITCH
PC3 ──┘
```

Fisicamente, temos uma estrutura em estrela.

---

## Topologia lógica

Representa **como os dados circulam ou como a comunicação acontece na rede**.

Ou seja:

> Física = como está conectado.

> Lógica = como a comunicação funciona.

Uma rede pode ter uma determinada topologia física e uma organização lógica diferente.

---

# 🧠 Não confunda topologia com classificação de rede

Você já estudou **classificação por abrangência**:

```text
PAN → LAN → CAN → MAN → WAN → GAN
```

Isso responde:

> **Qual é o alcance da rede?**

Topologia responde:

> **Como os dispositivos estão organizados/conectados?**

Por exemplo:

```text
LAN
└── Topologia em estrela
```

Uma LAN pode utilizar uma topologia em estrela.

---

# 🔗 Relação com o que você já estudou

Você já viu:

```text
Dispositivos
     ↓
Meios de transmissão
     ↓
Topologia
     ↓
Comunicação
     ↓
Protocolos
     ↓
IP / MAC
     ↓
Internet
```

Por exemplo:

```text
PC
 │
 │ Ethernet
 ↓
Switch
 │
 │ Ethernet
 ↓
Roteador
 │
 │
 ↓
Internet
```

Aqui você consegue relacionar vários assuntos:

- **Ethernet** → tecnologia de rede
- **Cabo** → meio de transmissão
- **Switch** → conecta dispositivos na rede local
- **MAC** → identificação na camada de enlace
- **IP** → endereçamento lógico
- **Roteador** → encaminha pacotes entre redes
- **Topologia** → organização das conexões

---

# ☕ Relação com programação

Isso também vai aparecer quando você começar Java.

Imagine:

```text
        Internet
           │
        Roteador
           │
        Switch
       /      \
      /        \
Frontend      Backend
              │
           Banco de
            Dados
```

Quando você desenvolver uma aplicação:

```text
Frontend
   ↓
HTTP/HTTPS
   ↓
Rede
   ↓
Servidor Java
   ↓
Banco de dados
```

Você não precisa ser especialista em redes para programar, mas entender essa estrutura vai fazer muito mais sentido quando você começar a trabalhar com **APIs, servidores, Spring Boot, banco de dados e aplicações web**.

---

# 🧠 O que realmente guardar

Não precisa decorar todos os detalhes históricos das topologias.

O principal é saber:

### Barramento
> Um meio principal compartilhado.

### Estrela
> Dispositivos conectados a um ponto central.

### Anel
> Dispositivos formando um circuito.

### Malha
> Vários caminhos/conexões entre dispositivos.

### Árvore
> Estrutura hierárquica.

### Híbrida
> Combinação de diferentes topologias.

E principalmente:

> **Topologia = forma como uma rede é organizada e conectada.**
