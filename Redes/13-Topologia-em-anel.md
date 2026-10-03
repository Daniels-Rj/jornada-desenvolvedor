# 🔄 Topologia em Anel (Ring)

## 📌 O que é?

Na **topologia em anel**, os dispositivos são conectados formando um **circuito fechado**.

Cada dispositivo normalmente possui conexão com os dispositivos vizinhos.

```text
        PC1
       /   \
     PC2   PC4
       \   /
        PC3
```

Ou de uma forma mais linear:

```text
PC1 ─── PC2
│         │
│         │
PC4 ─── PC3
```

O importante é que o último dispositivo se conecta novamente ao primeiro, formando um **anel**.

---

# 🔄 Como funciona?

Os dados circulam pelo anel de um dispositivo para outro.

Por exemplo:

```text
PC1 → PC2 → PC3
```

Se o PC1 precisa enviar informações para o PC3, os dados podem passar pelo PC2 até chegar ao destino.

```text
PC1
 ↓
PC2
 ↓
PC3
```

Dependendo da tecnologia utilizada, os dados podem circular em uma determinada direção.

---

# 🧠 Por que se chama anel?

Porque a estrutura forma um circuito fechado:

```text
       PC1
      /   \
    PC2   PC4
      \   /
       PC3
```

Não existe uma extremidade como no barramento.

```text
BARRAMENTO:

PC1 ─── PC2 ─── PC3 ─── PC4
↑                         ↑
└────── meio principal ───┘


ANEL:

      PC1
     /   \
   PC2   PC4
     \   /
      PC3
```

---

# 🔄 Sentido da transmissão

Uma rede em anel pode ser projetada para que os dados sigam um determinado sentido.

Por exemplo:

```text
PC1 → PC2 → PC3 → PC4 → PC1
```

Nesse caso, os dados seguem pelo anel nessa direção.

Algumas implementações utilizam mecanismos diferentes para aumentar a tolerância a falhas.

---

# 🎫 Token

Um conceito importante associado a algumas redes em anel é o **token**.

O token é uma espécie de "permissão para transmitir".

Imagine:

```text
PC1 → PC2 → PC3 → PC4 → PC1
```

O token circula pela rede.

Quando um dispositivo recebe o token e precisa transmitir:

```text
TOKEN → PC2
```

O PC2 pode utilizar a oportunidade para transmitir seus dados.

Depois, o mecanismo permite que o token continue circulando.

### Objetivo

Controlar quem pode transmitir e evitar que vários dispositivos transmitam ao mesmo tempo.

---

# ⚠️ E se um dispositivo falhar?

Em uma implementação simples:

```text
PC1 → PC2 → ❌ PC3 → PC4
```

Uma falha pode interromper o funcionamento do anel.

Isso é uma das desvantagens tradicionais dessa topologia.

Porém, existem implementações mais resistentes a falhas que utilizam caminhos redundantes ou anéis duplos.

---

# ✅ Vantagens

- Estrutura organizada.
- A comunicação pode ser controlada de maneira previsível.
- Algumas implementações utilizam token para controlar o acesso ao meio.
- Pode existir redundância em versões específicas, como anéis duplos.

---

# ❌ Desvantagens

- Uma falha pode afetar a comunicação em implementações simples.
- Alterar a rede pode ser mais complicado.
- Não é a topologia predominante nas redes Ethernet locais modernas.
- Diagnóstico e manutenção podem ser mais trabalhosos dependendo da implementação.

---

# ⭐ Comparando com as outras topologias

## 🚌 Barramento

```text
========================
 │       │       │
PC1     PC2     PC3
```

Um meio principal compartilhado.

---

## ⭐ Estrela

```text
       PC1
        │
PC2 ─ SWITCH ─ PC3
        │
       PC4
```

Um ponto central.

---

## 🔄 Anel

```text
      PC1
     /   \
   PC2   PC4
     \   /
      PC3
```

Um circuito fechado.

---

# 🧠 Uma forma fácil de memorizar

```text
🚌 BARRAMENTO
→ linha principal

⭐ ESTRELA
→ ponto central

🔄 ANEL
→ circuito fechado
```

---

# 🏠 E a rede da minha casa?

A sua rede doméstica, pelo que vimos anteriormente, **não é uma topologia em anel tradicional**.

Ela se aproxima mais de uma estrela:

```text
              ROTEADOR
             /   |   \
            /    |    \
          PC    TV   CELULAR
```

O roteador funciona como um ponto central de comunicação.

---

# 📌 O que realmente guardar

> **Topologia em anel = dispositivos conectados formando um circuito fechado.**

O conceito mais importante é visualizar:

```text
A → B → C → D
↑           ↓
└───────────┘
```

E lembrar que **anel não significa necessariamente que os dados sempre vão passar por todos os computadores**. O funcionamento exato depende da tecnologia e do protocolo utilizados.
