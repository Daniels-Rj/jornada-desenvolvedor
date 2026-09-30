# Internet, Intranet e Extranet

## 1. Introdução

Os termos **Internet**, **Intranet** e **Extranet** estão relacionados a redes de computadores, mas representam formas diferentes de disponibilizar e controlar o acesso a recursos de rede.

De forma resumida:

```text
INTERNET
↓
Rede pública e global

INTRANET
↓
Rede privada e interna de uma organização

EXTRANET
↓
Recursos privados disponibilizados para usuários externos autorizados
```

---

# 2. Internet

A **Internet** é uma enorme rede mundial formada pela interligação de diversas redes.

Ela conecta:

- Computadores
- Smartphones
- Servidores
- Data centers
- Empresas
- Provedores de Internet
- Redes domésticas
- Redes acadêmicas
- Redes governamentais
- Dispositivos IoT
- Entre muitos outros dispositivos e sistemas

Podemos pensar na Internet como uma **rede de redes**.

```text
Rede doméstica
       │
       ▼
Provedor
       │
       ▼
    Internet
       │
 ┌─────┼─────┐
 ▼     ▼     ▼
Web   APIs  Serviços
```

---

# 3. Características da Internet

A Internet possui algumas características importantes:

- É global;
- Interliga diversas redes;
- Utiliza protocolos de comunicação padronizados;
- Permite comunicação entre dispositivos de diferentes redes;
- Possui serviços públicos e privados;
- Não é controlada por uma única empresa ou computador.

Entre os protocolos e tecnologias utilizados na Internet estão:

- IP
- TCP
- UDP
- HTTP
- HTTPS
- DNS
- BGP
- Ethernet
- Wi-Fi
- Entre muitos outros.

---

# 4. Exemplos de serviços na Internet

Quando utilizamos:

- Google;
- YouTube;
- GitHub;
- Instagram;
- E-mail;
- Sites;
- APIs;
- Serviços de streaming;
- Jogos online;

estamos utilizando serviços que podem estar disponíveis através da Internet.

Uma comunicação pode seguir um caminho parecido com:

```text
Seu computador
      ↓
Roteador
      ↓
Provedor de Internet
      ↓
Internet
      ↓
Outras redes
      ↓
Servidor
```

---

# 5. Internet não significa apenas Web

É importante não confundir:

```text
Internet ≠ Web
```

A **Internet** é a infraestrutura e o conjunto de redes interconectadas.

A **Web (World Wide Web)** é um dos serviços que funciona sobre essa infraestrutura.

Podemos representar:

```text
                    INTERNET
                       │
        ┌──────────────┼──────────────┐
        ↓              ↓              ↓
       WEB            E-mail       Jogos online
        │
   HTTP / HTTPS
```

Portanto:

> **A Web utiliza a Internet, mas a Internet não se resume à Web.**

---

# 6. Intranet

A **Intranet** é uma rede ou conjunto de recursos de rede **privados de uma organização**, utilizados principalmente por seus funcionários ou usuários internos autorizados.

Exemplo:

```text
                 EMPRESA
                    │
        ┌───────────┼───────────┐
        ↓           ↓           ↓
       RH           TI      Financeiro
        │           │           │
        └───────────┼───────────┘
                    ↓
                 INTRANET
```

Uma empresa pode utilizar uma intranet para disponibilizar:

- Sistemas internos;
- Documentos;
- Comunicados;
- Sistemas de RH;
- Sistemas financeiros;
- Dashboards;
- Ferramentas corporativas;
- Bases de conhecimento;
- Sistemas administrativos.

---

# 7. Exemplo de Intranet

Imagine uma empresa com um sistema interno:

```text
http://intranet.empresa.local
```

Um funcionário conectado à rede da empresa pode acessar:

```text
Portal interno
      │
      ├── RH
      ├── Contracheque
      ├── Comunicados
      ├── Documentos
      └── Sistemas internos
```

Uma pessoa aleatória na Internet não deveria conseguir acessar esses recursos simplesmente conhecendo o endereço.

O acesso é controlado pela organização.

---

# 8. Intranet não significa necessariamente uma rede fisicamente separada

Uma intranet pode utilizar tecnologias semelhantes às utilizadas na Internet.

Por exemplo:

- TCP/IP
- HTTP/HTTPS
- DNS
- Ethernet
- Wi-Fi
- Servidores Web
- Bancos de dados
- APIs

A principal diferença está no **controle de acesso e no contexto em que os recursos são disponibilizados**.

Por isso, uma aplicação interna pode ser tecnicamente muito parecida com um site da Internet.

---

# 9. Extranet

A **Extranet** permite que determinados recursos privados de uma organização sejam disponibilizados para **usuários externos autorizados**.

Esses usuários podem ser:

- Fornecedores;
- Clientes;
- Parceiros;
- Prestadores de serviço;
- Distribuidores;
- Outras organizações.

Exemplo:

```text
                 EMPRESA
                    │
        ┌───────────┴───────────┐
        ↓                       ↓
    Funcionários            Parceiros
        ↓                       ↓
    INTRANET                EXTRANET
```

---

# 10. Exemplo de Extranet

Imagine uma empresa que trabalha com vários fornecedores.

Ela pode permitir que um fornecedor acesse um portal específico:

```text
Fornecedor
     │
     ▼
Portal da empresa
     │
     ▼
EXTRANET
     │
     ├── Consultar pedidos
     ├── Enviar documentos
     ├── Consultar entregas
     └── Consultar informações autorizadas
```

O fornecedor possui acesso a determinados recursos, mas isso **não significa que ele tenha acesso à rede interna inteira da empresa**.

---

# 11. Diferença entre Internet, Intranet e Extranet

| Característica | Internet | Intranet | Extranet |
|---|---|---|---|
| Alcance | Global | Interno | Interno + externos autorizados |
| Acesso | Público/aberto conforme o serviço | Restrito | Restrito |
| Usuários | Público em geral | Funcionários/usuários internos | Parceiros, clientes, fornecedores etc. |
| Objetivo | Comunicação e serviços globais | Recursos internos | Compartilhamento controlado com externos |
| Exemplo | Google | Portal interno da empresa | Portal de fornecedores |

---

# 12. Uma forma simples de memorizar

```text
INTERNET
↓
Mundo externo / rede global

INTRANET
↓
Dentro da organização

EXTRANET
↓
Organização + usuários externos autorizados
```

Outra forma:

```text
Internet
    │
    ├── Público
    │
    └── Global


Intranet
    │
    └── Funcionários / usuários internos


Extranet
    │
    ├── Organização
    │
    └── Parceiros externos autorizados
```

---

# 13. Comparando com uma empresa

Imagine uma empresa chamada:

```text
Empresa XYZ
```

Ela possui:

### Internet

Seu site público:

```text
www.empresaxyz.com
```

Qualquer pessoa pode acessar o conteúdo que a empresa disponibilizou publicamente.

```text
Cliente
   │
   ▼
Internet
   │
   ▼
Site da Empresa
```

---

### Intranet

Sistema interno:

```text
intranet.empresaxyz.local
```

Utilizado pelos funcionários:

```text
Funcionário
     │
     ▼
Intranet
     │
     ├── RH
     ├── Financeiro
     ├── Documentos
     └── Sistemas internos
```

---

### Extranet

Portal para fornecedores:

```text
portal.empresaxyz.com
```

Com acesso controlado:

```text
Fornecedor
     │
     ▼
Extranet
     │
     ├── Pedidos
     ├── Documentos
     └── Entregas
```

---

# 14. Segurança

A diferença entre Internet, Intranet e Extranet também envolve **controle de acesso e segurança**.

Uma organização pode utilizar mecanismos como:

- Firewall;
- Autenticação;
- Senhas;
- Controle de permissões;
- VPN;
- Criptografia;
- Certificados digitais;
- Controle de identidade;
- Segmentação de rede;
- Monitoramento.

Um exemplo simplificado:

```text
Internet
   │
   ▼
Firewall
   │
   ├───────────────┐
   ↓               ↓
Intranet         Extranet
   │               │
Funcionários    Externos autorizados
```

---

# 15. Firewall

Um **firewall** pode controlar o tráfego entre diferentes redes ou sistemas.

Por exemplo:

```text
Internet
    │
    ▼
┌───────────┐
│ FIREWALL  │
└─────┬─────┘
      │
      ▼
Rede interna
```

Ele pode aplicar regras para determinar quais conexões são permitidas ou bloqueadas.

---

# 16. VPN

Uma organização também pode utilizar uma **VPN (Virtual Private Network)** para permitir que usuários autorizados acessem recursos privados através de uma conexão protegida.

Exemplo:

```text
Funcionário em casa
        │
        │ VPN
        ▼
    Internet
        │
        ▼
   Firewall/VPN
        │
        ▼
Rede da empresa
        │
        ▼
    Intranet
```

Isso permite que um funcionário autorizado possa acessar determinados recursos internos mesmo estando fora da empresa.

---

# 17. Internet, Intranet e Extranet utilizam protocolos semelhantes

Um ponto importante é que os três conceitos não representam necessariamente tecnologias completamente diferentes.

Todos podem utilizar tecnologias como:

```text
TCP/IP
HTTP/HTTPS
DNS
Ethernet
Wi-Fi
```

Por exemplo, uma aplicação de intranet pode funcionar através de:

```text
HTTPS
   ↓
TCP
   ↓
IP
   ↓
Ethernet/Wi-Fi
```

Da mesma maneira que uma aplicação disponível na Internet.

A principal diferença está em **quem pode acessar os recursos e quais recursos estão disponíveis**.

---

# 18. Internet x Intranet

### Internet

```text
Usuários
   │
   ▼
Internet
   │
   ▼
Serviços públicos
```

### Intranet

```text
Funcionários
     │
     ▼
Rede privada
     │
     ▼
Sistemas internos
```

Podemos resumir:

> **Internet = rede global de redes.**

> **Intranet = recursos de rede privados voltados para usuários internos.**

---

# 19. Internet x Extranet

### Internet

Um serviço pode ser disponibilizado publicamente:

```text
Qualquer usuário
       ↓
   Internet
       ↓
Serviço público
```

### Extranet

O serviço é disponibilizado apenas para usuários externos autorizados:

```text
Parceiro autorizado
       ↓
   Internet
       ↓
Autenticação/controle
       ↓
   Extranet
```

Portanto:

> **Extranet não significa simplesmente "Internet para empresas".**

É o uso controlado de recursos privados para usuários externos autorizados.

---

# 20. Intranet x Extranet

Essa é provavelmente a comparação mais importante:

### Intranet

```text
Empresa
  │
  └── Funcionários
```

### Extranet

```text
Empresa
  │
  ├── Funcionários
  │
  └── Usuários externos autorizados
```

A principal diferença está no **público autorizado a acessar os recursos**.

---

# 21. Exemplo completo

Imagine uma empresa de comércio:

```text
                    EMPRESA
                       │
             ┌─────────┼─────────┐
             │         │         │
             ▼         ▼         ▼
           RH          TI     Financeiro
             │         │         │
             └─────────┼─────────┘
                       │
                    INTRANET
                       │
                       │
                 acesso controlado
                       │
                       ▼
                    EXTRANET
                       │
              ┌────────┼────────┐
              ▼        ▼        ▼
         Fornecedor Cliente Parceiro
```

Ao mesmo tempo, a empresa pode possuir um site público:

```text
                    INTERNET
                       │
                       ▼
                Site da empresa
                       │
                       ▼
                    Clientes
```

---

# 22. Relação com os conceitos estudados anteriormente

Essa aula se conecta diretamente com os conceitos anteriores.

Já estudamos:

```text
MAC
IP
Máscara
Gateway
DNS
TCP
HTTPS
Roteadores
Switches
Firewall
```

Agora podemos visualizar como eles podem fazer parte de uma rede corporativa:

```text
                    INTERNET
                       │
                       ▼
                    Firewall
                       │
              ┌────────┴────────┐
              │                 │
              ▼                 ▼
          INTRANET           EXTRANET
              │                 │
              ▼                 ▼
        Funcionários      Parceiros autorizados
```

Dentro dessas redes podem existir:

```text
IP
MAC
DNS
DHCP
TCP/IP
HTTP/HTTPS
Switches
Roteadores
```

---

# 23. Relação com programação

Esses conceitos também serão importantes quando começarmos a desenvolver sistemas.

Imagine uma empresa que possui um sistema desenvolvido em Java:

```text
             FRONT-END
                  │
                  │ HTTPS
                  ▼
             API REST
                  │
                  ▼
          Java / Spring Boot
                  │
                  ▼
             Banco de dados
```

Esse sistema pode ser disponibilizado:

### Publicamente

```text
Internet
   ↓
API
   ↓
Sistema
```

### Internamente

```text
Intranet
   ↓
API
   ↓
Sistema interno
```

### Para parceiros

```text
Extranet
   ↓
API
   ↓
Recursos autorizados
```

Isso mostra como os conceitos de redes estão diretamente relacionados ao desenvolvimento de software.

---

# 24. Resumo visual

```text
                    REDES
                      │
        ┌─────────────┼─────────────┐
        ↓             ↓             ↓
    INTERNET       INTRANET      EXTRANET
        │             │             │
        │             │             │
     Global        Interna       Externos
     Pública       Privada       autorizados
```

---

# 25. Resumo para memorizar

```text
INTERNET
→ Rede global de redes.

INTRANET
→ Rede/recursos privados utilizados internamente por uma organização.

EXTRANET
→ Recursos privados disponibilizados para usuários externos autorizados.
```

### Comparação:

```text
Internet
→ Público / global

Intranet
→ Interno / privado

Extranet
→ Externo autorizado / privado
```

---

# 26. Conceitos-chave

| Termo | Significado |
|---|---|
| **Internet** | Rede global formada pela interligação de diversas redes |
| **Intranet** | Rede ou conjunto de recursos privados de uma organização |
| **Extranet** | Recursos privados disponibilizados a usuários externos autorizados |
| **Firewall** | Controla o tráfego de rede de acordo com regras |
| **VPN** | Permite uma conexão virtual protegida a uma rede |
| **TCP/IP** | Conjunto de protocolos utilizado na comunicação em redes |
| **HTTP/HTTPS** | Protocolos utilizados principalmente na comunicação Web |
| **DNS** | Sistema que resolve nomes de domínio em endereços IP |

---

# 27. Conclusão

A diferença fundamental entre Internet, Intranet e Extranet está principalmente no **alcance, finalidade e controle de acesso**.

```text
INTERNET
↓
Rede global
↓
Serviços públicos

INTRANET
↓
Rede/recursos privados
↓
Usuários internos

EXTRANET
↓
Recursos privados
↓
Usuários externos autorizados
```

É importante lembrar que **Internet, Intranet e Extranet não são necessariamente três tecnologias completamente diferentes**.

Uma intranet ou extranet pode utilizar as mesmas tecnologias fundamentais da Internet, como:

```text
TCP/IP
HTTP/HTTPS
DNS
Ethernet
Wi-Fi
```

O que muda principalmente é:

```text
QUEM PODE ACESSAR?
        +
O QUE PODE ACESSAR?
        +
COMO O ACESSO É CONTROLADO?
```

> **Ideia principal:** a Internet conecta redes globalmente, a Intranet disponibiliza recursos de forma privada para usuários internos e a Extranet permite que determinados recursos privados sejam acessados por usuários externos autorizados.
