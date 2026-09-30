# Tipos de Rede: Ponto a Ponto e Cliente-Servidor

## 1. Introdução

Os computadores de uma rede precisam se comunicar e compartilhar recursos.

Existem diferentes formas de organizar essa comunicação.

Duas formas importantes são:

- **Rede Ponto a Ponto (Peer-to-Peer / P2P)**
- **Rede Cliente-Servidor**

A principal diferença está na forma como os computadores assumem seus papéis dentro da rede.

---

# 2. Rede Ponto a Ponto

Uma rede **Ponto a Ponto**, também chamada de **Peer-to-Peer (P2P)**, é uma rede na qual os computadores podem atuar diretamente uns com os outros.

Não existe necessariamente um servidor central responsável por todos os recursos.

Cada computador pode:

- Solicitar recursos;
- Fornecer recursos;
- Compartilhar arquivos;
- Compartilhar impressoras;
- Compartilhar informações.

Podemos representar:

```text
┌──────────┐
│ Computador│
│    A      │
└─────┬────┘
      │
      │
┌─────▼────┐
│ Computador│
│    B      │
└─────┬────┘
      │
      │
┌─────▼────┐
│ Computador│
│    C      │
└──────────┘
```

Os computadores podem se comunicar diretamente.

---

# 3. Por que o nome "Ponto a Ponto"?

O nome vem da ideia de que os dispositivos, chamados de **peers**, podem se comunicar diretamente entre si.

```text
Peer
  ↕
Peer
  ↕
Peer
```

Não existe necessariamente uma máquina central controlando todos os recursos.

---

# 4. Exemplo simples

Imagine três computadores em uma pequena empresa:

```text
PC A
 │
 ├── compartilha arquivos
 │
PC B
 │
 ├── compartilha arquivos
 │
PC C
```

O computador A pode disponibilizar uma pasta para B.

B pode disponibilizar outra pasta para A e C.

C também pode compartilhar seus próprios recursos.

Nesse modelo, os computadores podem assumir tanto o papel de quem **solicita** quanto de quem **fornece** determinado recurso.

---

# 5. Característica importante do Ponto a Ponto

No modelo P2P:

```text
Computador A
     ↕
Computador B
     ↕
Computador C
```

Os dispositivos podem atuar como:

```text
Cliente
   +
Servidor
```

Dependendo da situação.

Por isso, não devemos pensar que cada computador possui permanentemente um único papel.

---

# 6. Vantagens do Ponto a Ponto

### Simplicidade

Uma rede pequena pode ser criada sem a necessidade de um servidor dedicado.

### Baixo custo

Pode não ser necessário comprar e manter um servidor central.

### Fácil implementação

Em redes pequenas, pode ser relativamente simples compartilhar arquivos ou impressoras diretamente entre computadores.

---

# 7. Desvantagens do Ponto a Ponto

Conforme a rede cresce, podem aparecer problemas.

### Administração

Cada computador pode precisar ser configurado individualmente.

```text
PC A → configurações
PC B → configurações
PC C → configurações
PC D → configurações
...
```

### Segurança

O controle de acesso pode ficar mais difícil de administrar.

### Backup

Os arquivos podem estar espalhados por vários computadores.

### Escalabilidade

O modelo pode não ser adequado para redes corporativas grandes.

---

# 8. Quando P2P pode ser utilizado?

É mais comum encontrar esse modelo em:

- Redes pequenas;
- Ambientes domésticos;
- Compartilhamentos simples;
- Aplicações específicas de compartilhamento.

Também existem sistemas P2P na Internet, embora sejam diferentes de simplesmente compartilhar uma pasta entre computadores.

---

# 9. Cliente-Servidor

No modelo **Cliente-Servidor**, determinados computadores ou sistemas assumem funções específicas.

O:

```text
CLIENTE
```

faz solicitações.

O:

```text
SERVIDOR
```

fornece serviços ou recursos.

Representação:

```text
             SERVIDOR
                 │
        ┌────────┼────────┐
        │        │        │
        ▼        ▼        ▼
    Cliente   Cliente   Cliente
```

---

# 10. O que é um cliente?

O **cliente** é o dispositivo ou aplicação que solicita um serviço ou recurso.

Exemplos:

- Navegador;
- Aplicativo de celular;
- Programa de e-mail;
- Sistema empresarial;
- Aplicação Java;
- Aplicação desktop.

Por exemplo:

```text
Navegador
    │
    │ solicita página
    ▼
Servidor Web
```

Nesse caso:

```text
Navegador = Cliente
Servidor Web = Servidor
```

---

# 11. O que é um servidor?

Um **servidor** é um computador ou sistema que fornece algum serviço ou recurso para outros dispositivos ou aplicações.

Pode fornecer:

- Páginas Web;
- Arquivos;
- Banco de dados;
- E-mails;
- APIs;
- Autenticação;
- Serviços de rede;
- Aplicações.

Exemplo:

```text
Cliente
   │
   │ solicitação
   ▼
Servidor
   │
   │ resposta
   ▼
Cliente
```

---

# 12. Exemplo: acessar um site

Quando você abre um site:

```text
Você
 ↓
Navegador
 ↓
Internet
 ↓
Servidor Web
```

O navegador solicita um recurso.

Por exemplo:

```text
GET /index.html
```

O servidor processa a solicitação e envia uma resposta.

```text
Servidor
   ↓
HTML
CSS
JavaScript
Imagens
   ↓
Navegador
```

---

# 13. Exemplo: aplicativo do Instagram

Podemos simplificar:

```text
Aplicativo
     │
     │ solicitação
     ▼
   API
     │
     ▼
Servidor
     │
     ▼
Banco de dados
```

O aplicativo funciona como cliente.

O servidor fornece os dados e serviços necessários.

Por exemplo:

```text
Cliente
  ↓
"Quero minhas mensagens"
  ↓
Servidor
  ↓
Banco de dados
  ↓
Servidor
  ↓
Mensagens
  ↓
Cliente
```

---

# 14. Exemplo: banco de dados

Em uma empresa pode existir:

```text
Computadores dos funcionários
            │
            ▼
        Servidor
            │
            ▼
       Banco de dados
```

Os computadores dos funcionários podem solicitar informações ao servidor.

Por exemplo:

```text
Funcionário
     ↓
Sistema
     ↓
Servidor
     ↓
Banco de dados
     ↓
Servidor
     ↓
Sistema
     ↓
Funcionário
```

---

# 15. Vantagens do Cliente-Servidor

## Administração centralizada

Os recursos podem ser administrados em um local central.

```text
             SERVIDOR
                 │
       ┌─────────┼─────────┐
       ▼         ▼         ▼
     PC A       PC B      PC C
```

Isso facilita determinadas tarefas administrativas.

---

## Segurança centralizada

Permissões e autenticação podem ser administradas pelo servidor.

Por exemplo:

```text
Usuário
   ↓
Login
   ↓
Servidor
   ↓
Verificação
   ↓
Acesso permitido/negado
```

---

## Backup centralizado

Os dados importantes podem ser armazenados em servidores.

```text
PC A ──┐
PC B ──┼──→ Servidor
PC C ──┘       │
               ↓
             Backup
```

---

## Escalabilidade

É possível adicionar novos clientes ao ambiente.

```text
             SERVIDOR
                 │
       ┌─────────┼─────────┐
       ↓         ↓         ↓
      PC A      PC B      PC C
                           │
                           ↓
                          PC D
```

---

# 16. Desvantagens do Cliente-Servidor

### Custo

Pode ser necessário investir em:

- Servidores;
- Armazenamento;
- Rede;
- Backup;
- Segurança;
- Manutenção.

### Dependência do servidor

Se um serviço depende de um determinado servidor e esse servidor ficar indisponível:

```text
Servidor OFFLINE
      ↓
Serviço pode ficar indisponível
```

Por isso, sistemas importantes normalmente utilizam mecanismos de redundância e alta disponibilidade.

---

# 17. Comparação

| Característica | Ponto a Ponto | Cliente-Servidor |
|---|---|---|
| Organização | Descentralizada | Mais centralizada |
| Servidor dedicado | Não necessariamente | Normalmente existe |
| Administração | Distribuída | Centralizada |
| Custo inicial | Geralmente menor | Pode ser maior |
| Redes pequenas | Pode funcionar bem | Também pode funcionar |
| Redes grandes | Pode ficar difícil administrar | Mais adequado |
| Segurança | Mais distribuída | Pode ser centralizada |
| Backup | Pode ser distribuído | Pode ser centralizado |

---

# 18. Uma diferença fundamental

Podemos resumir:

### Ponto a Ponto

```text
PC A ↔ PC B
 ↕      ↕
PC C ↔ PC D
```

Os computadores podem fornecer e consumir recursos.

---

### Cliente-Servidor

```text
        SERVIDOR
       /   |   \
      /    |    \
    PC A  PC B  PC C
```

Existe uma separação mais clara entre:

```text
CLIENTE
   ↓
solicita

SERVIDOR
   ↓
fornece
```

---

# 19. Atenção: "servidor" não significa necessariamente um computador gigante

Um servidor é principalmente uma **função**.

Um computador comum pode executar um software servidor.

Por exemplo:

```text
Seu computador
      ↓
Executa um servidor Web
      ↓
Pode atender requisições
```

Nesse momento, aquele computador está desempenhando uma função de servidor.

---

# 20. Cliente também pode ser servidor

Esse conceito é especialmente importante no P2P.

Um mesmo computador pode:

```text
Solicitar arquivo
      ↓
CLIENTE
```

e também:

```text
Compartilhar arquivo
      ↓
SERVIDOR
```

Portanto:

> **Cliente e servidor representam papéis na comunicação, e não necessariamente tipos fixos de computadores.**

---

# 21. Um computador pode exercer várias funções

Um único computador pode executar vários serviços.

Por exemplo:

```text
Servidor
 ├── Web
 ├── Banco de dados
 ├── Arquivos
 └── Autenticação
```

Em sistemas maiores, essas funções podem ser separadas em diferentes servidores.

```text
              Rede
               │
      ┌────────┼────────┐
      ↓        ↓        ↓
   Web Server DB Server File Server
```

---

# 22. Relação com a Web

Quando você acessa um site:

```text
Navegador
   ↓
CLIENTE
   ↓
Internet
   ↓
SERVIDOR WEB
```

O navegador solicita:

```text
"Me envie esta página."
```

O servidor responde:

```text
"Aqui está a página."
```

---

# 23. Relação com APIs

Quando futuramente estudarmos **Java + Spring Boot**, veremos muito esse modelo.

Por exemplo:

```text
Frontend
   │
   │ HTTP/HTTPS
   ▼
API Java / Spring Boot
   │
   ▼
Banco de dados
```

Nesse cenário:

```text
Frontend = Cliente

Spring Boot = Servidor

Banco de dados = recurso utilizado pelo servidor
```

---

# 24. Relação com Full Stack

Isso será fundamental para entender Full Stack.

Uma aplicação pode ser organizada assim:

```text
┌─────────────────────┐
│      FRONT-END      │
│ HTML CSS JavaScript │
└──────────┬──────────┘
           │
           │ HTTP/HTTPS
           ▼
┌─────────────────────┐
│      BACK-END       │
│   Java / Spring     │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│      BANCO DE       │
│       DADOS         │
└─────────────────────┘
```

O usuário interage com o front-end.

O front-end faz solicitações ao back-end.

O back-end processa as solicitações e pode acessar o banco de dados.

---

# 25. Exemplo completo

Imagine um sistema de uma empresa.

Um funcionário quer consultar seu salário.

```text
Funcionário
     ↓
Navegador
     ↓
Front-end
     ↓
API
     ↓
Servidor Java
     ↓
Banco de dados
```

O banco retorna os dados:

```text
Banco de dados
     ↓
Servidor Java
     ↓
API
     ↓
Front-end
     ↓
Navegador
     ↓
Funcionário
```

Isso é um exemplo do modelo **Cliente-Servidor**.

---

# 26. P2P na Internet

P2P também pode existir em aplicações na Internet.

Em um sistema tradicional:

```text
Cliente → Servidor
```

No P2P:

```text
Computador A ↔ Computador B
      ↕             ↕
Computador C ↔ Computador D
```

Os próprios participantes podem fornecer recursos uns aos outros.

Um exemplo conhecido historicamente é o compartilhamento de arquivos utilizando protocolos P2P.

---

# 27. Conceito de Peer

A palavra:

> **Peer**

significa aproximadamente:

> **par / semelhante / participante do mesmo nível**

Em uma rede P2P:

```text
Peer A
  ↕
Peer B
  ↕
Peer C
```

Os participantes podem assumir funções semelhantes.

---

# 28. Resumo visual

```text
              TIPOS DE ORGANIZAÇÃO
                       │
             ┌─────────┴─────────┐
             │                   │
             ▼                   ▼
      PONTO A PONTO        CLIENTE-SERVIDOR
             │                   │
             ▼                   ▼
       Comunicação          Funções mais
       entre pares           separadas
             │                   │
             ▼                   ▼
        Peer ↔ Peer         Cliente → Servidor
```

---

# 29. O que preciso memorizar?

Não é necessário decorar uma lista enorme.

O principal é entender:

### Ponto a Ponto

```text
P2P

Computadores podem fornecer
e consumir recursos entre si.
```

### Cliente-Servidor

```text
Cliente

→ solicita recursos/serviços

Servidor

→ fornece recursos/serviços
```

### Conceito mais importante

```text
Cliente e servidor são PAPÉIS.

Não necessariamente computadores diferentes.
```

---

# 30. Resumo final

As redes podem organizar a comunicação de diferentes maneiras.

No modelo **Ponto a Ponto (P2P)**, os computadores podem se comunicar diretamente e assumir tanto o papel de cliente quanto de servidor.

```text
PC A ↔ PC B
PC C ↔ PC D
```

No modelo **Cliente-Servidor**, existe uma separação mais clara entre quem solicita e quem fornece determinado serviço.

```text
          SERVIDOR
         /   |   \
        ↓    ↓    ↓
      PC A  PC B  PC C
```

O modelo Cliente-Servidor é muito importante para entender:

- Sites;
- Aplicações Web;
- APIs;
- Sistemas empresariais;
- Bancos de dados;
- Aplicações Java;
- Spring Boot;
- Sistemas Full Stack.

> **Ideia principal:** Ponto a Ponto significa comunicação entre participantes que podem assumir papéis semelhantes; Cliente-Servidor significa uma organização em que clientes solicitam serviços e servidores fornecem esses serviços.
