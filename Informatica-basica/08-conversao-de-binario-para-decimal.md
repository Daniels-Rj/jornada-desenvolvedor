# 🔢 Conversão de Binário para Decimal

| Informação | Detalhes |
|---|---|
| 📚 **Curso** | Informática |
| 📖 **Módulo** | Sistemas de Numeração |
| 🎯 **Objetivo** | Aprender a converter números do sistema binário (base 2) para o sistema decimal (base 10), utilizando as potências de 2. |

---

## 📌 Binário → Decimal

O sistema **binário** utiliza apenas dois símbolos:

```text
0 e 1
```

Por isso, ele possui **base 2**.

O sistema **decimal**, que utilizamos no dia a dia, possui **base 10**:

```text
0 1 2 3 4 5 6 7 8 9
```

Na conversão de **binário para decimal**, utilizamos as **potências de 2** para descobrir o valor representado pelo número binário.

---

# 🧮 Tabela das Potências de 2

As posições do número binário correspondem às potências de 2.

```text
2⁴   2³   2²   2¹   2⁰
16    8    4    2    1
```

A posição mais à direita sempre começa em:

```text
2⁰ = 1
```

Depois seguimos para a esquerda:

```text
2¹ = 2
2² = 4
2³ = 8
2⁴ = 16
2⁵ = 32
2⁶ = 64
...
```

### 📊 Tabela básica

| Potência | Valor |
|---|---:|
| 2⁰ | 1 |
| 2¹ | 2 |
| 2² | 4 |
| 2³ | 8 |
| 2⁴ | 16 |
| 2⁵ | 32 |
| 2⁶ | 64 |
| 2⁷ | 128 |
| 2⁸ | 256 |
| 2⁹ | 512 |
| 2¹⁰ | 1024 |

---

# 🔄 Como converter Binário → Decimal?

Para realizar a conversão:

1. Monte a tabela das potências de 2.
2. Alinhe cada bit do número binário com uma potência de 2.
3. Observe quais posições possuem **1**.
4. Ignore as posições que possuem **0**.
5. Some os valores das posições que possuem **1**.

### 📌 Regra principal

```text
1 → utiliza o valor da potência de 2
0 → não utiliza o valor da potência de 2
```

---

# 🧮 Exemplo 1 — Binário 101 → Decimal

Vamos converter:

```text
101₂ → ?₁₀
```

Primeiro montamos a tabela:

```text
2²   2¹   2⁰
 4    2    1
```

Agora colocamos o número binário:

```text
Binário:   1    0    1
           ↓    ↓    ↓
Valor:     4    2    1
```

O número possui:

```text
1 → utiliza 4
0 → não utiliza 2
1 → utiliza 1
```

Então:

```text
4 + 1 = 5
```

Resultado:

```text
101₂ = 5₁₀
```

---

# 🧮 Exemplo 2 — Binário 1010 → Decimal

Vamos converter:

```text
1010₂ → ?₁₀
```

Tabela:

```text
2³   2²   2¹   2⁰
 8    4    2    1
```

Agora alinhamos:

```text
Binário:   1    0    1    0
           ↓    ↓    ↓    ↓
Valor:     8    4    2    1
```

Selecionamos apenas as posições com **1**:

```text
8 + 2 = 10
```

Resultado:

```text
1010₂ = 10₁₀
```

---

# 🧮 Exemplo 3 — Binário 1101 → Decimal

Vamos converter:

```text
1101₂ → ?₁₀
```

Tabela:

```text
2³   2²   2¹   2⁰
 8    4    2    1
```

Alinhando:

```text
Binário:   1    1    0    1
           ↓    ↓    ↓    ↓
Valor:     8    4    2    1
```

Selecionamos os valores correspondentes aos **1**:

```text
8 + 4 + 1 = 13
```

Resultado:

```text
1101₂ = 13₁₀
```

---

# 🧮 Exemplo 4 — Binário 11001 → Decimal

Agora um exemplo maior:

```text
11001₂ → ?₁₀
```

Tabela:

```text
2⁴   2³   2²   2¹   2⁰
16    8    4    2    1
```

Alinhando:

```text
Binário:   1    1    0    0    1
           ↓    ↓    ↓    ↓    ↓
Valor:    16    8    4    2    1
```

Selecionamos apenas os valores onde existe **1**:

```text
16 + 8 + 1
```

Calculando:

```text
16 + 8 + 1 = 25
```

Resultado:

```text
11001₂ = 25₁₀
```

---

# 🧮 Exemplo 5 — Binário 101010 → Decimal

Vamos converter:

```text
101010₂ → ?₁₀
```

Tabela:

```text
2⁵   2⁴   2³   2²   2¹   2⁰
32   16    8    4    2    1
```

Alinhando:

```text
Binário:   1    0    1    0    1    0
           ↓    ↓    ↓    ↓    ↓    ↓
Valor:    32   16    8    4    2    1
```

Selecionamos os valores com **1**:

```text
32 + 8 + 2
```

Calculando:

```text
32 + 8 + 2 = 42
```

Resultado:

```text
101010₂ = 42₁₀
```

---

# 📊 Comparando os dois métodos

Na aula anterior aprendemos:

```text
DECIMAL → BINÁRIO
```

Agora aprendemos:

```text
BINÁRIO → DECIMAL
```

### Decimal → Binário

Procuramos quais potências de 2 **formam o número**:

```text
25

16 + 8 + 1 = 25

16   8   4   2   1
 1   1   0   0   1

↓
11001
```

### Binário → Decimal

Pegamos as posições que possuem **1** e somamos seus valores:

```text
11001

16   8   4   2   1
 1   1   0   0   1

16 + 8 + 1 = 25
```

Portanto:

```text
25₁₀ = 11001₂

11001₂ = 25₁₀
```

---

# 🧠 Regra simples para lembrar

```text
BINÁRIO → DECIMAL

1 → pega o valor
0 → ignora o valor

Depois:
SOMA TUDO
```

### Exemplo:

```text
1  0  1  1
↓  ↓  ↓  ↓
8  4  2  1

1 → 8
0 → ignora 4
1 → 2
1 → 1

8 + 2 + 1 = 11
```

Logo:

```text
1011₂ = 11₁₀
```

---

# ⚠️ Erro comum

Não devemos simplesmente somar todos os valores da tabela.

Por exemplo:

```text
Binário:   1    0    1    0
Valor:     8    4    2    1
```

O correto é:

```text
8 + 2 = 10
```

E não:

```text
8 + 4 + 2 + 1
```

Porque o **0 significa que aquela posição não está sendo utilizada**.

---

# 🔍 Como conferir a conversão?

Podemos fazer o caminho inverso.

Por exemplo:

```text
1010₂ = 10₁₀
```

Agora podemos pegar o decimal:

```text
10
```

E verificar se conseguimos formar esse número com as potências de 2:

```text
8 + 2 = 10
```

Então:

```text
8   4   2   1
1   0   1   0

↓
1010
```

A conversão está correta.

---

# 📊 Exemplos para consultar

| Binário | Decimal |
|---:|---:|
| `0` | 0 |
| `1` | 1 |
| `10` | 2 |
| `11` | 3 |
| `100` | 4 |
| `101` | 5 |
| `110` | 6 |
| `111` | 7 |
| `1000` | 8 |
| `1001` | 9 |
| `1010` | 10 |
| `1011` | 11 |
| `1100` | 12 |
| `1101` | 13 |
| `1110` | 14 |
| `1111` | 15 |
| `10000` | 16 |
| `11001` | 25 |
| `101010` | 42 |

---

# 🔄 Resumo Visual

```text
             BINÁRIO
                ↓
       Separar cada posição
                ↓
       Associar às potências
              de 2
                ↓
       ┌────────┴────────┐
       ↓                 ↓
      1                  0
   utiliza             ignora
    valor               valor
       ↓                 ↓
       └────────┬────────┘
                ↓
              SOMAR
                ↓
             DECIMAL
```

---

## 🧠 O que preciso lembrar?

> O sistema binário utiliza apenas **0 e 1**.

> Para converter **binário → decimal**, utilizamos as **potências de 2**.

> Começamos pela direita com **2⁰ = 1**.

> Quando encontramos **1**, utilizamos o valor daquela posição.

> Quando encontramos **0**, ignoramos o valor daquela posição.

> No final, **somamos os valores das posições que possuem 1**.

### 🔑 Exemplo principal

```text
11001₂

2⁴   2³   2²   2¹   2⁰
16    8    4    2    1

 1    1    0    0    1

16 + 8 + 1 = 25

11001₂ = 25₁₀
```

---

## 📚 Próximos tópicos

- [x] Sistema decimal
- [x] Sistema binário
- [x] Potências de 2
- [x] Conversão de decimal para binário
- [x] Conversão de binário para decimal
- [x] Utilização da tabela de potências de 2
- [ ] Conversão entre outros sistemas
- [ ] Próximo tópico
