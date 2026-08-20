# 🖥️ Placa-Mãe

| Informação | Detalhes |
|---|---|
| 📚 **Curso** | Hardware |
| 📖 **Módulo** | Componentes do Computador |
| 🎯 **Objetivo** | Compreender a função da placa-mãe, suas principais características e os componentes que podem ser conectados a ela. |

---

# 🧩 O que é a Placa-Mãe?

A **placa-mãe (Motherboard)** é a principal placa de circuito de um computador.

Ela funciona como uma espécie de **estrutura central de comunicação**, permitindo que os diferentes componentes do computador sejam conectados e se comuniquem entre si.

Entre os componentes conectados à placa-mãe estão:

- Processador (CPU);
- Memória RAM;
- Placa de vídeo (GPU);
- SSDs;
- HDs;
- Placas de expansão;
- Dispositivos USB;
- Placa de rede;
- Dispositivos de áudio;
- Fonte de alimentação.

### 📌 Exemplo simplificado

```text
                    PLACA-MÃE
                        │
       ┌────────────────┼────────────────┐
       ↓                ↓                ↓
      CPU              RAM              GPU
       │                │                │
       └────────────────┼────────────────┘
                        │
                 Armazenamento
                  SSD / HDD
                        │
                        ↓
                Outros dispositivos
```

### 🧠 Para lembrar

> **Placa-mãe = principal placa do computador, responsável por conectar e permitir a comunicação entre seus componentes.**

---

# 🔌 Principais componentes e conexões

A placa-mãe possui diferentes **soquetes, slots, conectores e circuitos** destinados a diferentes funções.

Alguns dos mais importantes são:

```text
Placa-mãe
│
├── Socket da CPU
├── Slots de RAM
├── Slots PCI Express
├── Conectores SATA
├── Slots M.2
├── Conectores de energia
├── Portas USB
├── Conectores de áudio
└── Conectores de rede
```

---

# 🧠 Socket do Processador

O **socket** é o local da placa-mãe onde o processador é instalado.

```text
Placa-mãe
    │
    ↓
  Socket
    │
    ↓
   CPU
```

O socket precisa ser **compatível com o processador**.

Isso significa que não podemos simplesmente instalar qualquer CPU em qualquer placa-mãe.

### 📌 Exemplo

Um processador possui determinado padrão de socket.

A placa-mãe precisa possuir um socket compatível:

```text
CPU
 ↓
Socket compatível
 ↓
Placa-mãe
```

### 🧠 Para lembrar

> **Socket = local da placa-mãe onde o processador é instalado.**

---

# 💾 Slots de Memória RAM

A placa-mãe possui slots destinados à instalação dos módulos de **memória RAM**.

```text
Placa-mãe
    │
    ↓
Slots de RAM
    │
    ├── RAM
    ├── RAM
    └── RAM
```

A quantidade de slots depende do modelo da placa-mãe.

Também é necessário verificar a **compatibilidade da memória**, como o tipo e a geração suportada.

### 🧠 Para lembrar

> **Slots de RAM = locais onde os módulos de memória RAM são instalados.**

---

# 🎮 Slots PCI Express

Os **slots PCI Express (PCIe)** são utilizados para conectar diferentes dispositivos e placas de expansão.

Um dos usos mais conhecidos é a instalação de uma **placa de vídeo dedicada**.

### Exemplos de dispositivos

- Placas de vídeo;
- Placas de captura;
- Placas de som;
- Placas de rede;
- Outros dispositivos de expansão.

### 📌 Exemplo

```text
Placa-mãe
    │
    ↓
PCI Express
    │
    ↓
Placa de vídeo
```

### 🧠 Para lembrar

> **PCI Express = interface utilizada para conectar placas e dispositivos de expansão.**

---

# 💽 Conectores SATA

Os conectores **SATA** podem ser utilizados para conectar dispositivos de armazenamento, como:

- HDDs;
- SSDs SATA.

Exemplo:

```text
SSD SATA
    │
    │ Cabo SATA
    ↓
Placa-mãe
```

O SATA é uma interface de comunicação utilizada para conectar o dispositivo de armazenamento à placa-mãe.

---

# ⚡ Slots M.2

Algumas placas-mãe possuem slots **M.2**, utilizados principalmente para dispositivos como SSDs NVMe.

Exemplo:

```text
SSD NVMe
    │
    ↓
Slot M.2
    │
    ↓
Placa-mãe
```

Um SSD NVMe conectado via PCI Express pode apresentar velocidades muito superiores às de um SSD SATA, dependendo do modelo e da interface utilizada.

### ⚠️ Importante

**M.2 e NVMe não são exatamente a mesma coisa.**

```text
M.2
↓
Formato físico / conector

NVMe
↓
Protocolo de comunicação
```

Um dispositivo M.2 pode utilizar diferentes interfaces, embora SSDs NVMe em formato M.2 sejam muito comuns.

---

# 🔋 Conectores de Energia

A placa-mãe precisa receber energia da **fonte de alimentação (PSU)**.

A fonte fornece energia para a placa-mãe e para outros componentes do computador.

De forma simplificada:

```text
Fonte de alimentação
        ↓
    Placa-mãe
        ↓
 ┌──────┼──────┐
 ↓      ↓      ↓
 CPU    RAM    Outros componentes
```

O processador e outros componentes também possuem conexões específicas de energia.

---

# 🔌 Portas e Conectores

A placa-mãe também pode possuir diversas conexões para dispositivos externos.

Exemplos:

- USB;
- HDMI;
- DisplayPort;
- Ethernet;
- Áudio;
- PS/2 em alguns modelos.

### 📌 Exemplo

```text
Teclado
   ↓
USB
   ↓
Placa-mãe
```

Ou:

```text
Cabo de rede
      ↓
Porta Ethernet
      ↓
Placa-mãe
```

---

# 🌐 Placa de Rede Integrada

Muitas placas-mãe modernas já possuem uma **interface de rede integrada**.

Isso permite conectar o computador à rede sem necessariamente instalar uma placa de rede separada.

Exemplo:

```text
Placa-mãe
    │
    ↓
NIC integrada
    │
    ↓
Porta Ethernet
    │
    ↓
Roteador
```

Algumas placas-mãe também possuem **Wi-Fi integrado**.

---

# 🎧 Áudio Integrado

É comum que a placa-mãe possua recursos de áudio integrados.

Isso permite conectar dispositivos como:

- Fones de ouvido;
- Caixas de som;
- Microfones.

Em computadores modernos, normalmente não é necessário instalar uma placa de som separada para utilizar funções básicas de áudio.

---

# 🧠 Chipset

O **chipset** é um conjunto de componentes da placa-mãe responsável por auxiliar no gerenciamento da comunicação entre diferentes partes do sistema.

Ele influencia recursos como:

- Conectividade;
- Quantidade de portas e conexões;
- Recursos de expansão;
- Compatibilidade com determinados processadores e memórias;
- Recursos disponíveis na placa-mãe.

### 📌 Simplificando

```text
CPU
 │
 ├──────────────┐
 │              │
 ↓              ↓
RAM          Chipset
                │
       ┌────────┼────────┐
       ↓        ↓        ↓
     USB      SATA     PCIe
```

> O funcionamento exato depende da plataforma e da arquitetura utilizada.

---

# 🧩 Formato da Placa-Mãe

As placas-mãe possuem diferentes **formatos físicos (form factors)**.

Alguns exemplos:

- ATX;
- Micro-ATX;
- Mini-ITX.

O formato influencia características como:

- Tamanho da placa;
- Quantidade de slots;
- Quantidade de conectores;
- Compatibilidade com determinados gabinetes.

### 📊 Comparação simplificada

| Formato | Característica |
|---|---|
| **ATX** | Maior e geralmente possui mais possibilidades de expansão |
| **Micro-ATX** | Menor que ATX e ainda oferece boa expansão |
| **Mini-ITX** | Compacta, voltada para computadores menores |

### ⚠️ Importante

O formato da placa-mãe deve ser compatível com o gabinete.

```text
Placa-mãe
     ↓
Form factor
     ↓
Gabinete compatível
```

---

# 🔄 Como a Placa-Mãe conecta tudo?

A placa-mãe funciona como uma grande estrutura de conexão.

Imagine um computador:

```text
                    CPU
                     │
                     ↓
              ┌─────────────┐
              │             │
              │ PLACA-MÃE   │
              │             │
              └─────────────┘
               │     │     │
               ↓     ↓     ↓
              RAM   GPU   SSD
               │           │
               └─────┬─────┘
                     ↓
                Dados sendo
                processados
```

Os componentes não trabalham isoladamente.

A placa-mãe fornece as conexões e caminhos necessários para que eles possam **trocar dados e receber energia**.

---

# 🛠️ O que observar ao comprar uma placa-mãe?

Quando vamos escolher uma placa-mãe, não devemos olhar apenas para o preço.

É necessário verificar a compatibilidade e os recursos disponíveis.

### 🔎 Principais características

- Socket compatível com a CPU;
- Tipo e geração de memória RAM suportada;
- Quantidade de slots de RAM;
- Slots PCI Express;
- Quantidade de portas USB;
- Conectores SATA;
- Slots M.2;
- Recursos de rede;
- Wi-Fi integrado, quando disponível;
- Form factor;
- Recursos de expansão;
- Compatibilidade com o gabinete;
- Recursos de alimentação e suporte ao processador.

---

# 🎮 Exemplo prático

Imagine que você queira montar um computador para jogos.

Você possui:

```text
CPU
GPU
RAM
SSD
Fonte
```

A placa-mãe precisa oferecer os recursos necessários para conectar esses componentes.

```text
             PLACA-MÃE
                 │
     ┌───────────┼───────────┐
     ↓           ↓           ↓
    CPU         RAM         GPU
     │                       │
     └───────────┬───────────┘
                 ↓
                SSD
```

Por isso, a escolha da placa-mãe precisa considerar **todo o conjunto do computador**.

---

# 🧠 O que preciso lembrar?

> **Placa-mãe** é a principal placa de circuito do computador e conecta diversos componentes.

> **Socket** é o local onde o processador é instalado.

> **Slots de RAM** permitem instalar os módulos de memória.

> **PCI Express** é utilizado para conectar placas e dispositivos de expansão, como GPUs.

> **SATA** é uma interface utilizada para conectar dispositivos como HDDs e SSDs SATA.

> **M.2** é um formato de conexão utilizado por dispositivos como SSDs NVMe.

> **Chipset** participa do gerenciamento da comunicação e dos recursos disponíveis na plataforma.

> **ATX, Micro-ATX e Mini-ITX** são exemplos de formatos físicos de placas-mãe.

> Ao escolher uma placa-mãe, é necessário verificar a **compatibilidade entre CPU, RAM, armazenamento, gabinete e demais componentes**.

---

# 🔑 Resumo rápido

```text
🖥️ PLACA-MÃE
      ↓
Principal placa do computador
      ↓
Conecta os componentes
      │
      ├── CPU
      │     ↓
      │   Socket
      │
      ├── RAM
      │     ↓
      │   Slots de memória
      │
      ├── GPU
      │     ↓
      │   PCI Express
      │
      ├── SSD / HDD
      │     ↓
      │   SATA / M.2
      │
      ├── Rede
      │     ↓
      │   Ethernet / Wi-Fi
      │
      └── Periféricos
            ↓
          USB / Áudio
```

---

## 📚 Próximos tópicos

- [x] Função da placa-mãe
- [x] Socket da CPU
- [x] Slots de RAM
- [x] PCI Express
- [x] SATA
- [x] M.2
- [x] Chipset
- [x] Conectores de energia
- [x] Portas e conexões
- [x] Formatos ATX, Micro-ATX e Mini-ITX
- [x] Compatibilidade entre componentes
- [ ] Próximo tópico
