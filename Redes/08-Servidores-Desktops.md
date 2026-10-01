# Servidores e Desktops

## 1. Introdução

Um computador pode ser utilizado para diferentes finalidades.

Dois conceitos importantes são:

- **Desktop**
- **Servidor**

Apesar de ambos serem computadores e utilizarem componentes semelhantes, eles são projetados e configurados com **objetivos diferentes**.

Uma forma simples de entender:

```text
DESKTOP
↓
Computador voltado principalmente para uso do usuário.

SERVIDOR
↓
Computador voltado principalmente para fornecer serviços
e recursos para outros dispositivos ou aplicações.
```

---

# 2. O que é um Desktop?

**Desktop** é um computador destinado principalmente ao uso direto por uma pessoa.

Exemplos de atividades:

- Navegar na Internet;
- Estudar;
- Programar;
- Jogar;
- Editar imagens;
- Assistir vídeos;
- Utilizar programas;
- Trabalhar com documentos;
- Desenvolver sistemas.

Exemplo:

```text
             USUÁRIO
                ↓
             DESKTOP
                ↓
      ┌─────────┼─────────┐
      ↓         ↓         ↓
    Navegar   Programar   Jogar
```

---

# 3. Desktop não significa necessariamente "computador de mesa"

No uso cotidiano, muitas pessoas associam desktop a:

> "Computador que fica em cima da mesa."

Porém, no contexto de informática, **desktop** também pode se referir ao tipo de computador/ambiente voltado para interação direta com o usuário.

É importante diferenciar:

```text
Desktop PC
↓
Computador pessoal tradicional

Desktop environment
↓
Ambiente gráfico de um sistema operacional
```

Por exemplo:

- GNOME;
- KDE Plasma;
- XFCE.

No seu caso, por exemplo, você utiliza o **Zorin OS**, que possui uma interface gráfica baseada no GNOME.

---

# 4. Componentes de um Desktop

Um desktop normalmente possui:

```text
┌──────────────────────┐
│        CPU           │
│        RAM           │
│        SSD/HDD       │
│        GPU           │
│        Placa-mãe     │
└──────────────────────┘
          │
          ├── Monitor
          ├── Teclado
          ├── Mouse
          └── Outros periféricos
```

Os componentes podem variar bastante dependendo da finalidade.

Um computador para jogos, por exemplo, pode possuir uma GPU muito mais potente do que um computador destinado a tarefas de escritório.

---

# 5. O que é um Servidor?

Um **servidor** é um computador ou sistema que fornece algum serviço ou recurso para outros computadores, dispositivos ou aplicações.

Por exemplo:

```text
Cliente
   │
   │ solicitação
   ▼
SERVIDOR
   │
   │ resposta
   ▼
Cliente
```

O servidor pode fornecer:

- Sites;
- APIs;
- Arquivos;
- Banco de dados;
- E-mails;
- Sistemas;
- Autenticação;
- Serviços de rede;
- Armazenamento;
- Máquinas virtuais;
- Entre outros.

---

# 6. Servidor não é necessariamente um tipo especial de computador

Esse é um dos conceitos mais importantes.

Um servidor não é definido simplesmente pela aparência do computador.

Na prática:

> **Servidor é principalmente uma função que um computador ou sistema desempenha.**

Por exemplo, um computador comum pode executar um software de servidor Web.

```text
Computador
     ↓
Software servidor Web
     ↓
Recebe requisições
     ↓
Fornece páginas
```

Nesse momento, o computador está funcionando como um servidor Web.

---

# 7. Exemplo simples

Imagine seu próprio computador.

Se você estiver utilizando:

```text
Firefox
```

para acessar um site:

```text
Seu computador
      ↓
    Cliente
      ↓
   Internet
      ↓
Servidor Web
```

Seu computador está atuando como **cliente**.

Agora imagine que você instale um servidor Web no seu computador:

```text
Seu computador
      ↓
Servidor Web
      ↓
Recebe requisições
```

Agora ele também pode atuar como **servidor**.

---

# 8. Cliente e servidor são papéis

Isso conecta diretamente com a aula anterior.

```text
CLIENTE
↓
Solicita um serviço

SERVIDOR
↓
Fornece um serviço
```

Um mesmo computador pode exercer os dois papéis.

Por exemplo:

```text
Computador A
    │
    ├── Cliente de um serviço
    │
    └── Servidor de outro serviço
```

Portanto:

> **Cliente e servidor não significam necessariamente dois tipos diferentes de computador.**

---

# 9. Diferença de finalidade

A principal diferença entre um desktop e um servidor está na finalidade.

### Desktop

```text
Computador
     ↓
Usuário
     ↓
Aplicações
```

### Servidor

```text
Computador
     ↓
Serviços
     ↓
Outros computadores/aplicações
```

---

# 10. Servidores normalmente precisam ficar disponíveis

Um desktop normalmente é utilizado durante determinado período.

Por exemplo:

```text
08:00 → liga
18:00 → desliga
```

Um servidor que hospeda um site, por outro lado, pode precisar permanecer disponível continuamente.

```text
00:00 ─────────────── 24:00
       SERVIDOR
        ONLINE
```

Por isso, servidores importantes são projetados para oferecer alta disponibilidade.

---

# 11. Hardware de servidores

Servidores podem utilizar componentes semelhantes aos encontrados em desktops:

- CPU;
- RAM;
- SSD;
- HDD;
- Placa de rede;
- Placa-mãe;
- Fonte;
- GPU, quando necessária.

Porém, servidores podem utilizar componentes especificamente projetados para:

- Alta disponibilidade;
- Operação contínua;
- Grande quantidade de memória;
- Maior capacidade de armazenamento;
- Maior quantidade de conexões;
- Redundância;
- Facilidade de manutenção.

---

# 12. Processadores de servidores

Um servidor pode possuir processadores projetados para cargas de trabalho diferentes das encontradas em computadores pessoais.

Exemplo:

```text
Desktop
↓
Core i5 / Core i7 / Ryzen 5 / Ryzen 7

Servidor
↓
Xeon / EPYC / outros processadores de servidor
```

Isso não significa que um servidor obrigatoriamente precise de um processador específico.

Um computador comum também pode funcionar como servidor.

---

# 13. Memória RAM

Servidores podem precisar de grandes quantidades de RAM.

Por exemplo:

```text
Desktop:
8 GB
16 GB
32 GB

Servidor:
64 GB
128 GB
256 GB
512 GB
1 TB+
```

Os valores variam conforme a finalidade do servidor.

Um servidor de banco de dados, por exemplo, pode precisar de muita memória para trabalhar com grandes quantidades de dados.

---

# 14. Memória ECC

Servidores frequentemente utilizam memória **ECC (Error-Correcting Code)**.

A memória ECC possui mecanismos para detectar e, em determinadas situações, corrigir erros de memória.

Simplificando:

```text
RAM comum
↓
Armazena dados

RAM ECC
↓
Armazena dados
+
detecta determinados erros
+
pode corrigir determinados erros
```

Isso é importante em ambientes onde a confiabilidade é muito importante.

---

# 15. Armazenamento em servidores

Servidores podem utilizar:

- SSD;
- HDD;
- NVMe;
- Sistemas RAID;
- Armazenamento em rede.

Um servidor de arquivos, por exemplo, pode precisar de muitos terabytes de armazenamento.

```text
Servidor
   │
   ├── SSD
   ├── SSD
   ├── HDD
   └── HDD
```

---

# 16. RAID

**RAID** é uma tecnologia que combina vários dispositivos de armazenamento para obter características como:

- Redundância;
- Maior disponibilidade;
- Desempenho;
- Maior tolerância à falha.

Existem diferentes níveis de RAID.

Exemplos:

```text
RAID 0
RAID 1
RAID 5
RAID 6
RAID 10
```

Cada configuração possui características diferentes.

Importante:

> **RAID não substitui backup.**

RAID pode ajudar contra determinadas falhas de armazenamento, mas não protege automaticamente contra:

- Exclusão acidental;
- Ransomware;
- Corrupção lógica;
- Incêndio;
- Roubo;
- Outros desastres.

---

# 17. Fontes de alimentação

Servidores importantes podem utilizar fontes redundantes.

Por exemplo:

```text
        SERVIDOR
           │
      ┌────┴────┐
      ↓         ↓
   Fonte A    Fonte B
```

Se uma fonte apresentar problema, a outra pode manter o servidor funcionando, dependendo da configuração.

Isso é chamado de **redundância**.

---

# 18. Rede

Servidores normalmente possuem conexões de rede importantes.

Um servidor pode precisar atender:

```text
Cliente 1 ──┐
Cliente 2 ──┤
Cliente 3 ──┤
Cliente 4 ──┤
Cliente 5 ──┘
       ↓
    SERVIDOR
```

Por isso, servidores podem utilizar:

- Interfaces de rede de alta velocidade;
- Várias interfaces de rede;
- Conexões redundantes;
- Equipamentos de rede especializados.

---

# 19. Servidor não precisa ter monitor

Um desktop normalmente possui:

```text
Monitor
Teclado
Mouse
```

Um servidor pode funcionar sem esses periféricos conectados permanentemente.

Por exemplo:

```text
Servidor
   │
   └── Rede
        │
        └── Administrador
```

O administrador pode acessar o servidor remotamente.

---

# 20. Administração remota

Servidores frequentemente são administrados remotamente.

No Linux, um exemplo muito conhecido é:

```text
SSH
```

O administrador pode acessar:

```text
Seu computador
      │
      │ SSH
      ▼
Servidor Linux
```

E executar comandos remotamente.

Isso evita a necessidade de estar fisicamente diante do servidor.

---

# 21. Sistema operacional de servidor

Servidores podem utilizar diferentes sistemas operacionais.

Exemplos:

### Linux

Distribuições como:

- Ubuntu Server;
- Debian;
- Rocky Linux;
- AlmaLinux;
- Red Hat Enterprise Linux.

### Windows

- Windows Server.

O sistema escolhido depende da necessidade do ambiente.

---

# 22. Desktop x Servidor

| Característica | Desktop | Servidor |
|---|---|---|
| Objetivo principal | Uso do usuário | Fornecer serviços |
| Interface gráfica | Comum | Pode existir, mas não é obrigatória |
| Monitor | Normalmente utilizado | Pode não existir |
| Disponibilidade | Uso durante determinados períodos | Pode precisar funcionar continuamente |
| Hardware | Voltado ao uso pessoal | Pode ser voltado à confiabilidade e carga elevada |
| Manutenção | Normalmente local | Pode ser remota |
| Redundância | Menos comum | Comum em ambientes críticos |
| RAM | Conforme necessidade | Pode ser muito elevada |
| Armazenamento | Conforme necessidade | Pode ser muito grande |
| Rede | Geralmente uma conexão | Pode ter várias conexões |

---

# 23. Tipos de servidores

Existem diferentes tipos de servidores.

## Servidor Web

Fornece páginas e aplicações Web.

```text
Navegador
    ↓
Internet
    ↓
Servidor Web
    ↓
HTML / CSS / JS
```

Exemplos de software:

- Apache;
- Nginx;
- IIS.

---

# 24. Servidor de banco de dados

Responsável por fornecer acesso a bancos de dados.

```text
Aplicação
    ↓
Servidor
    ↓
Banco de dados
```

Exemplos de sistemas de banco de dados:

- MySQL;
- PostgreSQL;
- SQL Server;
- Oracle Database.

---

# 25. Servidor de arquivos

Fornece arquivos para usuários ou sistemas.

```text
PC A ──┐
PC B ──┼──→ Servidor de arquivos
PC C ──┘
```

Os usuários podem possuir permissões diferentes.

```text
João → leitura
Maria → leitura + escrita
Administrador → controle total
```

---

# 26. Servidor de e-mail

Pode fornecer serviços relacionados ao envio e recebimento de e-mails.

Exemplo conceitual:

```text
Usuário
   ↓
Cliente de e-mail
   ↓
Servidor de e-mail
   ↓
Internet
   ↓
Outro servidor
```

---

# 27. Servidor de DNS

O **DNS** transforma nomes de domínio em endereços IP.

Exemplo:

```text
www.exemplo.com
       ↓
      DNS
       ↓
192.0.2.10
```

Isso permite que as pessoas utilizem nomes em vez de precisar memorizar endereços IP.

---

# 28. Servidor DHCP

O **DHCP** pode fornecer configurações de rede automaticamente para dispositivos.

Por exemplo:

```text
Computador
    ↓
"Preciso de configuração de rede"
    ↓
DHCP
    ↓
IP
Máscara
Gateway
DNS
```

Em redes domésticas, essa função normalmente é realizada pelo roteador.

---

# 29. Servidor de aplicação

Um servidor de aplicação pode executar a lógica de uma aplicação.

Por exemplo:

```text
Front-end
    ↓
HTTP/HTTPS
    ↓
Servidor de aplicação
    ↓
Java / Spring Boot
    ↓
Banco de dados
```

Esse conceito será muito importante para você quando começar a estudar Java e Spring.

---

# 30. Servidor físico e servidor virtual

Um servidor pode ser:

### Físico

Um computador físico dedicado.

```text
┌───────────────────┐
│ Servidor físico   │
│                   │
│ CPU / RAM / SSD   │
└───────────────────┘
```

### Virtual

Uma máquina virtual executada dentro de outro computador físico.

```text
       SERVIDOR FÍSICO
             │
     ┌───────┼───────┐
     ↓       ↓       ↓
    VM1     VM2     VM3
```

Cada máquina virtual pode executar seu próprio sistema operacional.

---

# 31. Data Center

Muitos servidores são instalados em **data centers**.

Um data center é uma infraestrutura preparada para hospedar equipamentos de TI.

Pode possuir:

- Servidores;
- Roteadores;
- Switches;
- Sistemas de armazenamento;
- Climatização;
- Energia redundante;
- Geradores;
- Segurança física;
- Sistemas de monitoramento.

Representação:

```text
              DATA CENTER

      ┌──────────────────────┐
      │      Servidores      │
      │  █ █ █ █ █ █ █ █     │
      │  █ █ █ █ █ █ █ █     │
      │  █ █ █ █ █ █ █ █     │
      └──────────────────────┘
```

---

# 32. Desktop e servidor podem usar os mesmos conceitos fundamentais

Apesar das diferenças, ambos continuam sendo computadores.

Ambos podem possuir:

```text
CPU
RAM
Armazenamento
Placa-mãe
Sistema operacional
Rede
Software
```

A diferença principal está na:

```text
FINALIDADE
+
CONFIGURAÇÃO
+
CARGA DE TRABALHO
+
NÍVEL DE DISPONIBILIDADE
```

---

# 33. Exemplo usando seu computador

Seu VAIO é um exemplo de computador voltado para uso pessoal:

```text
VAIO
 │
 ├── Zorin OS
 ├── Navegador
 ├── Editor de código
 ├── Arquivos
 └── Aplicações
```

Ele pode funcionar como cliente:

```text
VAIO
 ↓
Firefox
 ↓
Servidor Web
```

Mas, se você instalar um servidor Web nele:

```text
VAIO
 ↓
Servidor Web
 ↓
Recebe requisições
```

ele também pode desempenhar uma função de servidor.

---

# 34. Um exemplo futuro com Java

Quando você desenvolver uma aplicação Full Stack:

```text
              USUÁRIO
                 ↓
             Navegador
                 ↓
              FRONT-END
                 ↓
              HTTPS
                 ↓
       SERVIDOR / API
                 ↓
         Java + Spring Boot
                 ↓
           Banco de dados
```

O computador onde o Java/Spring Boot está executando pode funcionar como um **servidor de aplicação**.

---

# 35. Conceito mais importante

Não pense:

```text
Servidor = computador gigante
Desktop = computador pequeno
```

Essa ideia está errada.

Pense:

```text
DESKTOP
→ finalidade principal: interação direta com usuário.

SERVIDOR
→ finalidade principal: fornecer serviços/recursos.
```

Um computador simples pode funcionar como servidor.

Um computador extremamente poderoso também pode ser utilizado como desktop.

---

# 36. Resumo final

### Desktop

É um computador destinado principalmente ao uso direto por uma pessoa.

```text
USUÁRIO
   ↓
DESKTOP
   ↓
APLICAÇÕES
```

### Servidor

É um computador ou sistema que fornece serviços ou recursos para outros dispositivos ou aplicações.

```text
CLIENTES
   ↓
SERVIDOR
   ↓
SERVIÇOS / RECURSOS
```

### Diferença fundamental

```text
Desktop
→ foco no usuário.

Servidor
→ foco em fornecer serviços.
```

> **Ideia principal:** servidor não é necessariamente um computador completamente diferente de um desktop. A diferença está principalmente na função, no software, na configuração e nos requisitos de disponibilidade, desempenho, confiabilidade e capacidade.
