# Cabos UTP e STP e Padrões de Cores

## 1. O que são cabos de par trançado?

Os cabos de **par trançado (Twisted Pair)** são cabos utilizados para transmissão de dados em redes, principalmente em redes Ethernet.

Eles possuem fios de cobre organizados em **pares**, e os fios de cada par são trançados entre si.

O trançamento ajuda a reduzir:

- interferências eletromagnéticas;
- ruídos;
- interferência entre os próprios pares.

---

# 2. UTP

**UTP = Unshielded Twisted Pair**

Em português:

> **Par Trançado Sem Blindagem**

É o tipo mais comum de cabo de rede utilizado em residências, empresas e redes Ethernet.

### Características

- Não possui blindagem metálica adicional.
- Possui pares de fios trançados.
- É mais simples e barato.
- É fácil de instalar e crimpar.
- É muito utilizado em redes Ethernet.

Exemplo:

```text
Computador ──── Cabo UTP ──── Switch
```

---

# 3. STP

**STP = Shielded Twisted Pair**

Em português:

> **Par Trançado Blindado**

Possui uma camada de blindagem para ajudar a proteger os sinais contra interferências eletromagnéticas.

É mais utilizado em ambientes onde existe maior possibilidade de interferência, como determinados ambientes industriais.

### Características

- Possui blindagem.
- Maior proteção contra interferências.
- Pode ser mais caro.
- A instalação é mais cuidadosa.
- A blindagem precisa ser corretamente aterrada quando o projeto exige isso.

---

# 4. UTP × STP

| Característica | UTP | STP |
|---|---|---|
| Blindagem | Não | Sim |
| Custo | Geralmente menor | Geralmente maior |
| Instalação | Mais simples | Mais complexa |
| Resistência a interferências | Menor | Maior |
| Uso comum | Residências e escritórios | Ambientes com maior interferência |

### Resumindo

```text
UTP → sem blindagem
STP → com blindagem
```

---

# 5. Estrutura de um cabo de rede

Um cabo Ethernet de par trançado possui normalmente **4 pares**, totalizando:

**8 condutores (fios)**.

Cada par possui dois fios.

```text
Par 1 → 2 fios
Par 2 → 2 fios
Par 3 → 2 fios
Par 4 → 2 fios

Total → 8 fios
```

Os fios possuem diferentes combinações de cores.

---

# 6. Padrões de cores

Existem dois padrões principais utilizados para organizar os fios no conector RJ-45:

- **T568A**
- **T568B**

Eles definem a ordem dos fios dentro do conector.

---

# 7. Padrão T568A

A ordem dos fios é:

```text
1 → Branco/Verde
2 → Verde
3 → Branco/Laranja
4 → Azul
5 → Branco/Azul
6 → Laranja
7 → Branco/Marrom
8 → Marrom
```

---

# 8. Padrão T568B

A ordem dos fios é:

```text
1 → Branco/Laranja
2 → Laranja
3 → Branco/Verde
4 → Azul
5 → Branco/Azul
6 → Verde
7 → Branco/Marrom
8 → Marrom
```

A principal diferença entre A e B está na troca dos pares:

```text
Verde ↔ Laranja
```

---

# 9. Cabo direto (Straight-Through)

Quando utilizamos o **mesmo padrão nas duas pontas**, temos um cabo direto.

Exemplo:

```text
T568B ───────────── T568B
```

ou:

```text
T568A ───────────── T568A
```

O importante é que as duas pontas utilizem o **mesmo padrão**.

---

# 10. Cabo crossover

Quando utilizamos padrões diferentes nas duas pontas:

```text
T568A ───────────── T568B
```

temos um cabo **crossover (cruzado)**.

Historicamente, esse tipo de cabo era utilizado para conectar determinados dispositivos diretamente, como:

```text
Computador ↔ Computador
Switch ↔ Switch
```

Porém, muitos equipamentos modernos possuem **Auto MDI-X**, que detecta automaticamente a configuração necessária.

Por isso, cabos crossover são muito menos necessários atualmente.

---

# 11. RJ-45

É comum ouvir:

> "conector RJ-45"

Ele é o conector modular normalmente utilizado nos cabos Ethernet de par trançado.

Exemplo:

```text
Cabo de rede
     │
     ▼
┌─────────────┐
│  RJ-45      │
└─────────────┘
```

Os 8 fios são posicionados em uma ordem específica dentro do conector.

---

# 12. Por que existe uma ordem de cores?

A ordem não existe simplesmente para deixar o cabo organizado.

Ela padroniza a maneira como os pares são conectados aos equipamentos.

Isso permite que diferentes fabricantes e profissionais possam montar e utilizar cabos seguindo o mesmo padrão.

---

# 13. O que preciso memorizar?

Para o nível de redes que estamos estudando agora, é importante saber:

### UTP

> **Unshielded Twisted Pair = par trançado sem blindagem.**

### STP

> **Shielded Twisted Pair = par trançado com blindagem.**

### Padrões

```text
T568A
T568B
```

### T568A

```text
Branco/Verde
Verde
Branco/Laranja
Azul
Branco/Azul
Laranja
Branco/Marrom
Marrom
```

### T568B

```text
Branco/Laranja
Laranja
Branco/Verde
Azul
Branco/Azul
Verde
Branco/Marrom
Marrom
```

### Regra principal

```text
Mesmo padrão nas duas pontas
        ↓
     Cabo direto

A de um lado + B do outro
        ↓
   Cabo crossover
```

---

# 14. Ligação com o que já estudamos

Esse assunto conecta vários conceitos anteriores:

```text
Meio de transmissão
       ↓
Cabo de par trançado
       ↓
UTP / STP
       ↓
Padrão T568A / T568B
       ↓
Conector RJ-45
       ↓
Ethernet
       ↓
Switch
       ↓
Comunicação através de MAC
```

Ou seja, agora você está começando a sair da parte mais conceitual de redes e entrando também na parte **física/prática**.

## 🧠 Mentalidade para guardar

> **UTP/STP dizem como o cabo é construído.**
>
> **T568A/T568B dizem como os fios são organizados nas pontas.**
>
> **RJ-45 é o conector utilizado na extremidade.**
>
> **Ethernet é uma das principais tecnologias que utiliza esses cabos em redes locais.**
