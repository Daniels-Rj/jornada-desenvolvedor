# 🖥️ Hardware — Placa de Rede, NIC, HDD e SSD

| Informação | Detalhes |
|---|---|
| 📚 **Curso** | Hardware |
| 📖 **Módulo** | Componentes do Computador |
| 🎯 **Objetivo** | Compreender o funcionamento básico das interfaces de rede e as diferenças entre HDD e SSD. |

---

# 🌐 Placa de Rede

A **placa de rede** é um componente responsável por permitir que o computador **se conecte e se comunique com uma rede**.

Ela possibilita a comunicação do computador com outros dispositivos, como:

- Roteadores;
- Switches;
- Servidores;
- Outros computadores;
- Impressoras de rede;
- Internet.

A conexão pode ser realizada de diferentes formas, principalmente:

```text
🔌 Rede cabeada
      ↓
Cabo Ethernet

📡 Rede sem fio
      ↓
Wi-Fi
```

### 📌 Exemplo

Quando um computador acessa um site:

```text
Computador
    ↓
Placa de rede
    ↓
Roteador
    ↓
Internet
    ↓
Servidor
```

A placa de rede participa da comunicação entre o computador e a rede.

---

# 🪪 NIC — Network Interface Card

**NIC** significa:

> **Network Interface Card**

Em português:

> **Placa de Interface de Rede**

Também podemos encontrar o termo:

> **Network Interface Controller**

A NIC é a **interface que permite ao dispositivo se conectar a uma rede**.

Na prática, o termo **NIC** pode ser utilizado para se referir à placa ou interface de rede responsável pela comunicação.

---

# 🔌 NIC Cabeada

Uma interface de rede Ethernet permite conectar o computador a uma rede utilizando um cabo.

Exemplo:

```text
Computador
    │
    │ Cabo Ethernet
    ↓
Roteador
    ↓
Internet
```

As interfaces Ethernet normalmente utilizam conectores como:

```text
RJ-45
```

### 📌 Vantagens da conexão cabeada

- Maior estabilidade;
- Baixa latência;
- Boa velocidade;
- Menor interferência que conexões sem fio em muitos ambientes.

---

# 📡 NIC Wi-Fi

Também existem interfaces de rede sem fio.

Nesse caso, o computador pode se conectar à rede utilizando **Wi-Fi**, sem precisar de um cabo Ethernet.

```text
Computador
    │
    │ Wi-Fi
    ↓
Roteador
    ↓
Internet
```

Notebooks normalmente já possuem uma interface Wi-Fi integrada.

Computadores de mesa também podem possuir Wi-Fi integrado à placa-mãe ou utilizar uma placa/adaptador Wi-Fi separado.

---

# 🧠 Endereço MAC

Uma interface de rede possui um identificador chamado **endereço MAC**.

**MAC** significa:

> **Media Access Control**

O endereço MAC é utilizado para identificar uma interface de rede no nível de enlace da rede.

Um endereço MAC é normalmente representado em hexadecimal.

### 📌 Exemplo

```text
00:1A:2B:3C:4D:5E
```

### ⚠️ MAC × IP

É importante não confundir:

```text
MAC
↓
Identifica a interface de rede

IP
↓
Identifica o endereço do dispositivo em uma rede
```

O endereço MAC está associado à interface de rede, enquanto o endereço IP é utilizado para identificar e localizar o dispositivo dentro de uma rede.

---

# 💽 Armazenamento

Além dos componentes responsáveis pela comunicação, os computadores possuem dispositivos destinados ao **armazenamento de dados**.

Dois exemplos muito conhecidos são:

```text
HDD
SSD
```

Ambos podem ser utilizados para armazenar:

- Sistema operacional;
- Programas;
- Jogos;
- Fotos;
- Vídeos;
- Documentos;
- Arquivos.

Porém, funcionam de maneiras diferentes.

---

# 💿 HDD

**HDD** significa:

> **Hard Disk Drive**

Em português:

> **Unidade de Disco Rígido**

O HDD utiliza **discos magnéticos e componentes mecânicos** para armazenar e acessar dados.

### 🧩 Funcionamento simplificado

```text
      HDD
       │
       ├── Pratos magnéticos
       │
       ├── Motor
       │
       └── Cabeça de leitura/gravação
```

Os pratos giram enquanto uma cabeça de leitura/gravação acessa os dados armazenados.

---

## ⚙️ Características do HDD

### ✅ Vantagens

- Grande capacidade de armazenamento;
- Geralmente possui menor custo por GB;
- Útil para armazenar grandes quantidades de arquivos.

### ❌ Desvantagens

- Possui partes mecânicas móveis;
- É mais lento que um SSD em muitos cenários;
- Pode produzir ruído;
- É mais sensível a impactos físicos enquanto está funcionando.

### 🧠 Para lembrar

> **HDD = armazenamento magnético com componentes mecânicos.**

---

# ⚡ SSD

**SSD** significa:

> **Solid State Drive**

Em português:

> **Unidade de Estado Sólido**

O SSD utiliza **memória flash** para armazenar dados e não possui os mesmos componentes mecânicos móveis presentes em um HDD.

### 🧩 Funcionamento simplificado

```text
        SSD
         │
         ↓
   Memória Flash
         │
         ↓
      Dados
```

---

## ⚙️ Características do SSD

### ✅ Vantagens

- Alta velocidade;
- Baixa latência;
- Não possui partes mecânicas móveis;
- Operação silenciosa;
- Melhor resistência a impactos físicos em comparação com HDDs.

### ❌ Desvantagens

- Geralmente possui custo maior por GB em comparação com HDDs;
- Possui limites de gravação, embora os SSDs modernos sejam projetados para suportar muitos anos de uso normal.

### 🧠 Para lembrar

> **SSD = armazenamento baseado em memória flash, sem partes mecânicas móveis.**

---

# ⚖️ HDD × SSD

| Característica | 💿 HDD | ⚡ SSD |
|---|---|---|
| Tecnologia | Magnética | Memória Flash |
| Partes móveis | ✅ Sim | ❌ Não |
| Velocidade | Menor | Maior |
| Latência | Maior | Menor |
| Ruído mecânico | Pode existir | Silencioso |
| Resistência a impactos | Menor | Maior |
| Custo por GB | Geralmente menor | Geralmente maior |
| Uso comum | Grande armazenamento | Sistema, programas e jogos |

---

# 🚀 Exemplo prático

Imagine dois computadores.

### Computador A — HDD

```text
Ligar computador
      ↓
HDD procura os arquivos
      ↓
Sistema operacional é carregado
      ↓
Computador inicia
```

### Computador B — SSD

```text
Ligar computador
      ↓
SSD acessa os dados
      ↓
Sistema operacional é carregado
      ↓
Computador inicia mais rapidamente
```

A diferença de velocidade é especialmente perceptível em tarefas como:

- Inicialização do sistema;
- Abertura de programas;
- Carregamento de jogos;
- Transferência de arquivos;
- Acesso a grandes quantidades de dados.

---

# 🧠 Por que o SSD é mais rápido?

O HDD precisa movimentar componentes mecânicos para encontrar os dados.

```text
HDD

Prato gira
   ↓
Cabeça se movimenta
   ↓
Localiza os dados
   ↓
Lê os dados
```

O SSD não precisa realizar esses movimentos mecânicos.

```text
SSD

Controlador
    ↓
Memória Flash
    ↓
Dados
```

Isso reduz bastante o tempo necessário para acessar os dados.

---

# 🔗 Relação entre os componentes

Agora podemos juntar os conceitos:

```text
                  COMPUTADOR
                      │
        ┌─────────────┴─────────────┐
        ↓                           ↓
    PROCESSAMENTO              COMUNICAÇÃO
        │                           │
       CPU                         NIC
        │                           │
        ↓                           ↓
       RAM                    Rede / Internet
        │
        ↓
    ARMAZENAMENTO
        │
     ┌──┴──┐
     ↓     ↓
    SSD   HDD
```

Cada componente possui uma função diferente:

```text
CPU
↓
Processa informações

RAM
↓
Armazena temporariamente dados em uso

NIC
↓
Permite comunicação com redes

SSD / HDD
↓
Armazenam dados de forma persistente
```

---

# 🧠 O que preciso lembrar?

> **Placa de rede** é o componente que permite ao computador se conectar e se comunicar com uma rede.

> **NIC** significa *Network Interface Card* e representa a interface responsável pela conexão do dispositivo com uma rede.

> Uma NIC pode fornecer conexão **cabeada (Ethernet)** ou **sem fio (Wi-Fi)**.

> **MAC** é um endereço associado à interface de rede.

> **HDD** utiliza discos magnéticos e componentes mecânicos para armazenar dados.

> **SSD** utiliza memória flash e não possui partes mecânicas móveis.

> **SSDs geralmente são muito mais rápidos que HDDs**, principalmente em acesso aos dados.

---

# 🔑 Resumo rápido

```text
🌐 NIC
↓
Interface de rede
↓
Permite comunicação com redes
↓
Ethernet / Wi-Fi


💿 HDD
↓
Disco magnético
↓
Possui partes mecânicas
↓
Maior latência


⚡ SSD
↓
Memória Flash
↓
Sem partes mecânicas móveis
↓
Menor latência
↓
Maior velocidade
```

---

## 📚 Próximos tópicos

- [x] Placa de rede
- [x] NIC — Network Interface Card
- [x] Ethernet
- [x] Wi-Fi
- [x] Endereço MAC
- [x] HDD
- [x] SSD
- [x] Diferenças entre HDD e SSD
- [ ] Próximo tópico
