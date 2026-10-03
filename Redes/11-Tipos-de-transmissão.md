# Tipos de Transmissão — Simplex, Half-Duplex e Full-Duplex

## 📌 O que são?

Esses três tipos classificam **como os dados podem trafegar entre dois dispositivos**, considerando a direção da comunicação.

A pergunta principal é:

> **Quem pode transmitir e em que momento?**

Existem três tipos principais:

- Simplex
- Half-Duplex
- Full-Duplex

---

# ➡️ 1. Simplex

No **Simplex**, a comunicação acontece em **apenas uma direção**.

Um dispositivo transmite e o outro apenas recebe.

```text
A ───────────→ B
```

O dispositivo B não envia dados de volta pelo mesmo canal de comunicação.

### Exemplos

Um exemplo clássico é uma **transmissão de televisão tradicional**:

```text
Emissora ─────────→ TV
```

A emissora transmite e a TV recebe.

Outro exemplo conceitual:

```text
Sensor ─────────→ Sistema
```

O sensor envia informações, mas não recebe informações pelo canal.

### Resumindo

> **Simplex = só vai.**

```text
A → B
```

---

# 🔄 2. Half-Duplex

No **Half-Duplex**, os dois dispositivos podem transmitir e receber, **mas não ao mesmo tempo**.

```text
A ─────────→ B
A ←───────── B
```

A comunicação acontece nos dois sentidos, mas cada lado precisa esperar sua vez.

### Exemplo clássico: Walkie-talkie

```text
Pessoa A: "Câmbio."
        ↓
Pessoa B recebe.

Pessoa B: "Pode falar."
        ↓
Pessoa A recebe.
```

Enquanto A fala, B espera.

Depois B fala e A espera.

### Resumindo

> **Half-Duplex = vai e volta, mas um de cada vez.**

```text
A → B
A ← B
```

---

# ↔️ 3. Full-Duplex

No **Full-Duplex**, os dois dispositivos podem transmitir e receber **ao mesmo tempo**.

```text
A ─────────→ B
A ←───────── B
```

As duas direções podem funcionar simultaneamente.

### Exemplo

Uma ligação telefônica tradicional:

```text
Pessoa A ─────────→ Pessoa B
Pessoa A ←───────── Pessoa B
```

A pode falar enquanto B também fala.

Outro exemplo comum:

### Ethernet moderna

Em conexões Ethernet **full-duplex**, o dispositivo pode transmitir e receber simultaneamente.

```text
Computador
    ↕
  Switch
```

---

# 📊 Comparação

| Tipo | Transmite | Recebe | Ao mesmo tempo? |
|---|---|---|---|
| Simplex | Sim | Não | ❌ |
| Half-Duplex | Sim | Sim | ❌ |
| Full-Duplex | Sim | Sim | ✅ |

---

# 🧠 Forma fácil de memorizar

### Simplex

```text
→
```

**Só uma direção.**

---

### Half-Duplex

```text
→
←
```

**Duas direções, mas uma por vez.**

---

### Full-Duplex

```text
↔
```

**Duas direções simultaneamente.**

---

# ⚠️ Não confundir com Unicast, Broadcast e Multicast

São classificações diferentes.

### Simplex / Half-Duplex / Full-Duplex

Pergunta:

> **Como a comunicação acontece nos sentidos de transmissão?**

```text
Simplex    → uma direção
Half-Duplex → duas direções, alternadamente
Full-Duplex → duas direções simultaneamente
```

### Unicast / Broadcast / Multicast

Pergunta:

> **Para quem os dados estão sendo enviados?**

```text
Unicast    → um destinatário
Broadcast  → todos
Multicast  → um grupo
```

Portanto, não são conceitos concorrentes.

Uma comunicação pode ser analisada pelas duas características.

---

# 🔗 Relação com redes

Imagine seu computador conectado a um switch:

```text
PC ───────── SWITCH
```

Em uma conexão **full-duplex**, podem acontecer simultaneamente:

```text
PC ─────────→ SWITCH
PC ←───────── SWITCH
```

Enquanto o computador envia dados, ele também pode receber dados.

Isso é importante para entender o funcionamento das redes Ethernet modernas.

---

# 🧠 O que guardar da aula

Não precisa decorar exemplos específicos.

O mais importante é entender:

```text
SIMPLEX
→ somente uma direção

HALF-DUPLEX
↔ duas direções
   mas uma por vez

FULL-DUPLEX
↔ duas direções
   simultaneamente
```

### Frase para lembrar:

> **Simplex só vai. Half-Duplex vai e volta, mas espera. Full-Duplex vai e volta ao mesmo tempo.**
