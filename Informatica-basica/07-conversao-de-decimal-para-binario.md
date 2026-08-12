# 🔢 Conversão de Decimal para Binário

| Informação | Detalhes |
|---|---|
| 📚 **Curso** | Informática |
| 📖 **Módulo** | Sistemas de Numeração |
| 🎯 **Objetivo** | Aprender a converter números do sistema decimal (base 10) para o sistema binário (base 2), utilizando a tabela de potências de 2. |

---

## 📌 Decimal → Binário

O sistema **decimal** é o sistema que utilizamos normalmente no dia a dia e possui **base 10**.

```text
0 1 2 3 4 5 6 7 8 9
```

O sistema **binário** possui **base 2** e utiliza somente dois símbolos:

```text
0 e 1
```

Na conversão de decimal para binário, podemos utilizar uma **tabela baseada nas potências de 2**.

---

# 🧮 Potências de 2

Cada posição de um número binário representa uma potência de 2.

A tabela começa pela direita com **2⁰**:

```text
2⁴   2³   2²   2¹   2⁰
 ↓    ↓    ↓    ↓    ↓
16    8    4    2    1
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

### 🧠 Para lembrar

> Cada posição do número binário representa uma **potência de 2**.

---

# 🔄 Como converter Decimal → Binário?

Para realizar a conversão utilizando a tabela:

1. Monte uma sequência de potências de 2.
2. Comece pela maior potência que não ultrapasse o número.
3. Verifique se cada valor pode ser utilizado.
4. Se utilizar o valor, coloque **1**.
5. Se não utilizar, coloque **0**.
6. Continue até chegar ao **1 (2⁰)**.

```text
Número decimal
      ↓
Tabela de potências de 2
      ↓
Escolher os valores necessários
      ↓
1 = utiliza
0 = não utiliza
      ↓
Número binário
```

---

# 🧮 Exemplo 1 — Decimal 5 → Binário

Queremos converter:

```text
5₁₀ → ?₂
```

Primeiro montamos a tabela:

```text
2²   2¹   2⁰
 4    2    1
```

Agora precisamos formar o número **5**.

```text
4 + 1 = 5
```

Então utilizamos **4** e **1**, mas não utilizamos **2**.

```text
Valor:     4   2   1
           ↓   ↓   ↓
Utiliza?   1   0   1
```

Resultado:

```text
5₁₀ = 101₂
```

---

# 🧮 Exemplo 2 — Decimal 10 → Binário

Queremos converter:

```text
10₁₀ → ?₂
```

Montamos a tabela:

```text
2³   2²   2¹   2⁰
 8    4    2    1
```

Precisamos formar o número **10**.

```text
8 + 2 = 10
```

Portanto:

```text
Valor:     8   4   2   1
           ↓   ↓   ↓   ↓
Utiliza?   1   0   1   0
```

Resultado:

```text
10₁₀ = 1010₂
```

### 🔎 Conferindo

```text
1 × 8 = 8
0 × 4 = 0
1 × 2 = 2
0 × 1 = 0

8 + 0 + 2 + 0 = 10
```

---

# 🧮 Exemplo 3 — Decimal 13 → Binário

Queremos converter:

```text
13₁₀ → ?₂
```

Tabela:

```text
2³   2²   2¹   2⁰
 8    4    2    1
```

Precisamos formar **13**:

```text
8 + 4 + 1 = 13
```

Então:

```text
Valor:     8   4   2   1
           ↓   ↓   ↓   ↓
Utiliza?   1   1   0   1
```

Resultado:

```text
13₁₀ = 1101₂
```

---

# 🧮 Exemplo 4 — Decimal 25 → Binário

Agora vamos utilizar um número um pouco maior:

```text
25₁₀ → ?₂
```

Montamos a tabela:

```text
2⁴   2³   2²   2¹   2⁰
16    8    4    2    1
```

Precisamos formar **25**.

Começamos pelo maior valor possível:

```text
25 - 16 = 9
```

Então utilizamos **16**.

Agora:

```text
9 - 8 = 1
```

Utilizamos **8**.

Não conseguimos utilizar **4**:

```text
1 < 4
```

Então colocamos **0**.

Também não conseguimos utilizar **2**:

```text
1 < 2
```

Então colocamos **0**.

Por fim, utilizamos **1**:

```text
1 - 1 = 0
```

Tabela final:

```text
Valor:     16   8   4   2   1
           ↓    ↓   ↓   ↓   ↓
Utiliza?    1    1   0   0   1
```

Resultado:

```text
25₁₀ = 11001₂
```

### 🔎 Conferindo

```text
1 × 16 = 16
1 × 8  = 8
0 × 4  = 0
0 × 2  = 0
1 × 1  = 1

16 + 8 + 0 + 0 + 1 = 25
```

---

# 🧮 Exemplo 5 — Decimal 42 → Binário

Agora um exemplo utilizando uma tabela maior:

```text
42₁₀ → ?₂
```

Tabela:

```text
2⁵   2⁴   2³   2²   2¹   2⁰
32   16    8    4    2    1
```

Formando 42:

```text
42 - 32 = 10
10 - 8 = 2
2 - 2 = 0
```

Não utilizamos 16, 4 ou 1.

```text
Valor:     32   16   8   4   2   1
           ↓    ↓    ↓   ↓   ↓   ↓
Utiliza?    1    0    1   0   1   0
```

Resultado:

```text
42₁₀ = 101010₂
```

### 🔎 Conferindo

```text
1 × 32 = 32
0 × 16 = 0
1 × 8  = 8
0 × 4  = 0
1 × 2  = 2
0 × 1  = 0

32 + 8 + 2 = 42
```

---

# 📊 Tabela de Exemplos

| Decimal | Potências utilizadas | Binário |
|---:|---|---:|
| 1 | 1 | `1` |
| 2 | 2 | `10` |
| 3 | 2 + 1 | `11` |
| 4 | 4 | `100` |
| 5 | 4 + 1 | `101` |
| 6 | 4 + 2 | `110` |
| 7 | 4 + 2 + 1 | `111` |
| 8 | 8 | `1000` |
| 9 | 8 + 1 | `1001` |
| 10 | 8 + 2 | `1010` |
| 11 | 8 + 2 + 1 | `1011` |
| 12 | 8 + 4 | `1100` |
| 13 | 8 + 4 + 1 | `1101` |
| 14 | 8 + 4 + 2 | `1110` |
| 15 | 8 + 4 + 2 + 1 | `1111` |
| 16 | 16 | `10000` |
| 25 | 16 + 8 + 1 | `11001` |
| 42 | 32 + 8 + 2 | `101010` |

---

# 💡 O que significa 1 e 0 na tabela?

Durante a conversão:

```text
1 = utiliza aquela potência de 2
0 = não utiliza aquela potência de 2
```

Por exemplo:

```text
Valor:     16   8   4   2   1
           ↓    ↓   ↓   ↓   ↓
Binário:    1    1   0   0   1
```

Isso significa:

```text
16 + 8 + 1 = 25
```

Portanto:

```text
11001₂ = 25₁₀
```

---

# 🧠 Por que usamos potências de 2?

O sistema binário possui **base 2**, portanto suas posições são baseadas nas potências de 2.

```text
2⁴   2³   2²   2¹   2⁰
 ↓    ↓    ↓    ↓    ↓
16    8    4    2    1
```

Cada posição representa um valor que pode ser:

```text
0 → não utilizar
1 → utilizar
```

Por isso, um número binário pode ser interpretado como uma combinação de potências de 2.

---

# 🔍 Exemplo visual

Considere:

```text
11001₂
```

Podemos separar cada posição:

```text
1    1    0    0    1
↓    ↓    ↓    ↓    ↓
16   8    4    2    1
```

Os valores que possuem **1** são utilizados:

```text
16 + 8 + 1 = 25
```

Logo:

```text
11001₂ = 25₁₀
```

---

# ⚠️ Erros comuns

### ❌ Confundir a ordem das potências

A tabela deve começar pela direita com:

```text
2⁰ = 1
```

E continuar:

```text
2¹ = 2
2² = 4
2³ = 8
2⁴ = 16
...
```

---

### ❌ Esquecer o zero

Se uma potência não for utilizada, precisamos colocar **0** naquela posição.

Por exemplo, 25:

```text
16 + 8 + 1
```

Não podemos escrever apenas:

```text
111
```

Precisamos manter todas as posições:

```text
16   8   4   2   1
 ↓   ↓   ↓   ↓   ↓
 1   1   0   0   1
```

Resultado:

```text
11001
```

---

# 🔄 Método em uma única sequência

```text
NÚMERO DECIMAL
      ↓
Montar tabela de potências de 2
      ↓
Encontrar os valores que formam o número
      ↓
1 = utiliza
0 = não utiliza
      ↓
Ler os 0 e 1 da esquerda para a direita
      ↓
NÚMERO BINÁRIO
```

---

## 🧠 O que preciso lembrar?

> Para converter **decimal para binário**, podemos utilizar uma tabela de **potências de 2**.

> As potências de 2 começam em **2⁰ = 1** e aumentam para a esquerda.

> **1** significa que aquela potência de 2 está sendo utilizada.

> **0** significa que aquela potência de 2 não está sendo utilizada.

> Para encontrar o binário, devemos escolher as potências de 2 que, somadas, formam o número decimal.

### 🔑 Exemplo principal

```text
25₁₀

16 + 8 + 1 = 25

Valor:     16   8   4   2   1
           ↓    ↓   ↓   ↓   ↓
Binário:    1    1   0   0   1

25₁₀ = 11001₂
```

---

## 📚 Próximos tópicos

- [x] Sistema decimal
- [x] Sistema binário
- [x] Potências de 2
- [x] Conversão de decimal para binário
- [x] Utilização da tabela de potências de 2
- [x] Representação por 0 e 1
- [ ] Conversão de binário para decimal
- [ ] Conversão entre outros sistemas
