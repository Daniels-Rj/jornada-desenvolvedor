# 🔢 Sistemas de Numeração

| Informação | Detalhes |
|---|---|
| 📚 **Curso** | Informática |
| 📖 **Módulo** | Conceitos Fundamentais |
| 🎯 **Objetivo** | Compreender o conceito de sistemas de numeração e conhecer os principais sistemas utilizados na computação. |

---

## 📌 O que é um Sistema de Numeração?

Um **sistema de numeração** é um conjunto de símbolos e regras utilizado para **representar valores numéricos**.

Diferentes sistemas utilizam diferentes quantidades de símbolos para representar os números.

Os principais sistemas estudados na computação são:

- 🔢 Decimal
- 💻 Binário
- 🧮 Octal
- 🧩 Hexadecimal

---

# 🔢 Sistema Decimal

O **sistema decimal** é o sistema de numeração que utilizamos normalmente no nosso dia a dia.

Ele possui **10 símbolos**, chamados de algarismos:

```text
0 1 2 3 4 5 6 7 8 9
```

Por isso, dizemos que o sistema decimal possui **base 10**.

### 📌 Exemplos

```text
10
25
100
350
2026
```

Esses números estão representados no sistema decimal.

### 🧠 Para lembrar

> **Decimal = base 10 = utiliza os algarismos de 0 a 9.**

---

# 💻 Sistema Binário

O **sistema binário** é um sistema de numeração fundamental para a computação.

Ele possui apenas **2 símbolos**:

```text
0 e 1
```

Por isso, possui **base 2**.

Os computadores digitais utilizam o sistema binário para representar e processar informações.

### 📌 Exemplos

```text
0
1
10
11
100
101
110
111
```

Um número binário pode representar diferentes informações dentro de um sistema computacional.

### 🧠 Para lembrar

> **Binário = base 2 = utiliza apenas 0 e 1.**

---

# 🧮 Sistema Octal

O **sistema octal** possui **8 símbolos**:

```text
0 1 2 3 4 5 6 7
```

Por isso, possui **base 8**.

O sistema octal foi utilizado em algumas aplicações relacionadas à computação, principalmente como uma forma mais compacta de representar números binários.

### 📌 Exemplos

```text
7
10
25
100
157
```

⚠️ O algarismo **8 não existe no sistema octal**.

### 🧠 Para lembrar

> **Octal = base 8 = utiliza os algarismos de 0 a 7.**

---

# 🧩 Sistema Hexadecimal

O **sistema hexadecimal** possui **16 símbolos**.

Como os algarismos de 0 a 9 não são suficientes para representar os 16 valores, utilizamos também as letras:

```text
0 1 2 3 4 5 6 7 8 9 A B C D E F
```

As letras representam os valores:

| Hexadecimal | Decimal |
|---|---:|
| **A** | 10 |
| **B** | 11 |
| **C** | 12 |
| **D** | 13 |
| **E** | 14 |
| **F** | 15 |

Por isso, o sistema hexadecimal possui **base 16**.

### 📌 Exemplos

```text
A
10
1F
FF
2A
```

O sistema hexadecimal é muito utilizado na computação porque permite representar grandes sequências binárias de maneira mais compacta.

### 🎨 Exemplo na programação

As cores utilizadas em **HTML e CSS** podem ser representadas utilizando hexadecimal:

```text
#FF0000
```

Nesse caso, o hexadecimal é utilizado para representar uma cor.

### 🧠 Para lembrar

> **Hexadecimal = base 16 = utiliza 0–9 e A–F.**

---

# 📊 Comparação dos Sistemas

| Sistema | Base | Símbolos utilizados |
|---|---:|---|
| 🔢 **Decimal** | 10 | 0–9 |
| 💻 **Binário** | 2 | 0–1 |
| 🧮 **Octal** | 8 | 0–7 |
| 🧩 **Hexadecimal** | 16 | 0–9 e A–F |

---

# 🔗 Relação entre os Sistemas

Os sistemas de numeração podem representar **o mesmo valor utilizando símbolos diferentes**.

Por exemplo, o número decimal **10** pode ser representado em diferentes sistemas:

```text
Decimal:      10
Binário:     1010
Octal:         12
Hexadecimal:    A
```

Apesar das representações serem diferentes, todas representam **o mesmo valor**.

### 🧠 Importante

> O que muda entre os sistemas é a **forma de representar o valor**, de acordo com a base utilizada.

---

# 🔢 O que significa "Base"?

A **base** indica quantos símbolos diferentes o sistema utiliza antes de começar uma nova posição numérica.

### Exemplos:

```text
Decimal → Base 10
10 símbolos → 0 até 9

Binário → Base 2
2 símbolos → 0 e 1

Octal → Base 8
8 símbolos → 0 até 7

Hexadecimal → Base 16
16 símbolos → 0 até 9 + A até F
```

---

# 📍 Valor Posicional

Nos sistemas de numeração, a posição de cada algarismo influencia seu valor.

No sistema decimal:

```text
5.432
```

Cada posição possui um peso diferente:

```text
5 × 1000
4 × 100
3 × 10
2 × 1
```

Ou:

```text
5 × 10³
4 × 10²
3 × 10¹
2 × 10⁰
```

O mesmo princípio existe em outros sistemas, mas utilizando suas respectivas bases.

### 📌 Exemplo no binário

```text
1011
```

As posições representam potências de 2:

```text
1 × 2³
0 × 2²
1 × 2¹
1 × 2⁰
```

---

# 💻 Por que o Binário é tão importante?

Os computadores digitais trabalham internamente com componentes eletrônicos que podem representar **dois estados distintos**.

Esses estados podem ser representados de forma simplificada como:

```text
0 → desligado
1 → ligado
```

Por isso, o sistema binário é adequado para representar informações em computadores digitais.

### 📌 Exemplo

```text
0 = OFF
1 = ON
```

Essa representação binária pode ser utilizada para construir informações muito mais complexas.

```text
Bits
 ↓
Bytes
 ↓
Dados
 ↓
Informações
```

---

# 🧩 Por que usar Hexadecimal?

Sequências binárias podem ficar muito grandes e difíceis de visualizar.

Por isso, o hexadecimal pode ser utilizado como uma representação mais compacta.

### Exemplo:

```text
Binário:

11111111
```

Pode ser representado em hexadecimal como:

```text
FF
```

Assim:

```text
11111111₂ = FF₁₆
```

Isso torna determinadas representações muito mais fáceis de ler.

---

# 🧠 O que preciso lembrar?

> **Sistema de numeração** é um conjunto de símbolos e regras utilizado para representar valores.

> **Decimal** possui base 10 e utiliza os algarismos de 0 a 9.

> **Binário** possui base 2 e utiliza apenas 0 e 1.

> **Octal** possui base 8 e utiliza os algarismos de 0 a 7.

> **Hexadecimal** possui base 16 e utiliza os algarismos de 0 a 9 e as letras A até F.

> O **binário** é fundamental para os computadores digitais.

> O **hexadecimal** permite representar sequências binárias de maneira mais compacta.

> A **base** determina a quantidade de símbolos disponíveis no sistema de numeração.

---

## 📚 Próximos tópicos

- [x] Conceito de sistemas de numeração
- [x] Sistema decimal
- [x] Sistema binário
- [x] Sistema octal
- [x] Sistema hexadecimal
- [x] Base de um sistema de numeração
- [x] Valor posicional
- [x] Relação entre os sistemas
- [ ] Conversão entre sistemas de numeração
- [ ] Próximo tópico
