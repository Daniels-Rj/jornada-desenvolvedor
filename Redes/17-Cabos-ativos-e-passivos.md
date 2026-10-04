# Equipamentos de Rede: Passivos e Ativos

## 1. O que são equipamentos de rede?

São componentes utilizados para construir, organizar, conectar e fazer uma rede funcionar.

Eles podem ser classificados, de forma geral, em:

- **Equipamentos passivos**
- **Equipamentos ativos**

A principal diferença está em saber se o equipamento **precisa atuar eletricamente/eletronicamente sobre o sinal ou sobre a comunicação**.

---

# 2. Equipamentos passivos

Os equipamentos passivos são componentes que fazem parte da infraestrutura física da rede, mas não realizam processamento ativo dos dados como um switch ou roteador.

Eles normalmente servem para:

- conectar cabos;
- organizar a infraestrutura;
- distribuir fisicamente os cabos;
- proteger e acomodar componentes;
- permitir a conexão física entre equipamentos.

### Exemplos

- Patch panel
- Rack
- Keystone
- Patch cord
- Tomada de rede
- Canaletas
- Organizadores de cabos
- Cabos de rede
- Conectores

---

# 3. Patch Panel

O **patch panel** é utilizado para organizar as conexões dos cabos de uma rede.

Ele normalmente fica instalado em um **rack**.

Exemplo:

```text
Computadores
     │
     │
Cabos da rede
     │
     ▼
┌──────────────────┐
│   PATCH PANEL    │
└──────────────────┘
          │
          │ Patch cords
          ▼
┌──────────────────┐
│     SWITCH       │
└──────────────────┘
```

O patch panel facilita:

- organização;
- identificação dos cabos;
- manutenção;
- alteração das conexões.

---

# 4. Rack

O **rack** é uma estrutura utilizada para acomodar equipamentos de rede e outros equipamentos de infraestrutura.

Pode conter:

- switches;
- patch panels;
- roteadores;
- servidores;
- organizadores;
- equipamentos de segurança;
- nobreaks.

Exemplo:

```text
┌─────────────────────┐
│      PATCH PANEL    │
├─────────────────────┤
│       SWITCH        │
├─────────────────────┤
│    ORGANIZADOR      │
├─────────────────────┤
│       ROUTER        │
└─────────────────────┘
        RACK
```

O rack em si não processa os dados.

Ele serve principalmente para **acomodar e organizar os equipamentos**.

---

# 5. Keystone

O **keystone** é um módulo utilizado para terminar/conectar cabos de rede em tomadas e painéis.

Pode ser utilizado, por exemplo, em:

```text
Parede
   │
   ▼
┌───────────────┐
│   Keystone    │
│   RJ-45       │
└───────────────┘
   │
   ▼
Computador
```

---

# 6. Patch Cord

O **patch cord** é um cabo de rede utilizado para realizar conexões entre equipamentos ou entre um equipamento e uma tomada/patch panel.

Exemplo:

```text
Patch Panel
     │
     │ Patch Cord
     ▼
   Switch
```

Normalmente é um cabo curto e flexível.

---

# 7. Equipamentos ativos

Os equipamentos ativos são dispositivos que possuem componentes eletrônicos e participam ativamente da comunicação da rede.

Eles podem:

- receber dados;
- processar dados;
- encaminhar dados;
- controlar tráfego;
- conectar redes diferentes;
- fornecer acesso à rede.

### Exemplos

- Switch
- Roteador
- Access Point
- Modem/ONT
- Firewall
- Repetidor
- Hub

---

# 8. Switch

O **switch** conecta dispositivos dentro de uma rede local.

Ele utiliza principalmente os **endereços MAC** para encaminhar quadros para a porta apropriada.

Exemplo:

```text
PC 1 ───┐
PC 2 ───┤
PC 3 ───┤── Switch
PC 4 ───┘
```

O switch é um dos equipamentos mais importantes de uma **LAN**.

---

# 9. Roteador

O **roteador (router)** conecta redes diferentes e encaminha pacotes com base em endereços IP e informações de roteamento.

Exemplo:

```text
LAN
 │
 │
 ▼
ROTEADOR
 │
 │
 ▼
Internet
```

Em uma residência, o roteador geralmente também pode oferecer:

- Wi-Fi;
- DHCP;
- NAT;
- firewall;
- outras funções.

Por isso, aquele equipamento fornecido pela operadora pode desempenhar várias funções ao mesmo tempo.

---

# 10. Access Point

O **Access Point (AP)** fornece acesso à rede através de uma conexão sem fio.

Ele permite que dispositivos como:

- notebooks;
- celulares;
- tablets;
- TVs;

se conectem à rede utilizando Wi-Fi.

Exemplo:

```text
        📱
         \
💻 ─── Wi-Fi ─── Access Point ─── Switch
         /
       📺
```

---

# 11. Modem / ONT

Dependendo da tecnologia utilizada pela operadora, existe um equipamento responsável pela interface com o meio de acesso.

Em uma conexão de fibra óptica, por exemplo, é comum existir uma **ONT/ONU**, que realiza a interface entre a rede óptica da operadora e a rede do cliente.

Em outras tecnologias, pode existir um modem.

É importante não tratar "modem" e "roteador" como sinônimos:

```text
Modem/ONT
   ↓
Interface com a tecnologia de acesso

Roteador
   ↓
Encaminhamento entre redes
```

Um único equipamento doméstico pode combinar várias dessas funções.

---

# 12. Hub

O **hub** é um equipamento de rede mais antigo.

Quando recebe um sinal em uma porta, ele normalmente o repete para as outras portas.

```text
       PC 1
         │
         ▼
      ┌─────┐
PC 2 ─│ HUB │─ PC 3
      └─────┘
         │
        PC 4
```

Diferentemente de um switch moderno, o hub não toma decisões com base no endereço MAC para encaminhar o quadro somente à porta necessária.

Por isso, os hubs foram amplamente substituídos pelos switches nas redes Ethernet modernas.

---

# 13. Repetidor

O repetidor recebe um sinal e o retransmite para aumentar o alcance de uma transmissão.

Conceito:

```text
Sinal
  ↓
Origem ─────── Repetidor ─────── Destino
                   ↓
             retransmite
```

Ele é utilizado para ajudar a superar limitações de alcance do meio de transmissão.

---

# 14. Firewall

O firewall controla o tráfego de rede de acordo com regras de segurança.

Pode permitir ou bloquear determinadas comunicações.

```text
Internet
   │
   ▼
FIREWALL
   │
   ▼
Rede interna
```

Firewalls podem existir em:

- roteadores;
- computadores;
- servidores;
- equipamentos dedicados;
- ambientes corporativos.

---

# 15. Passivo × Ativo

| Característica | Passivo | Ativo |
|---|---|---|
| Atua eletronicamente na comunicação | Não, em geral | Sim |
| Processa/encaminha dados | Não | Sim |
| Precisa de alimentação elétrica | Geralmente não | Geralmente sim |
| Exemplos | Rack, patch panel, cabos | Switch, roteador, AP |
| Função principal | Infraestrutura física | Comunicação/processamento |

> **Atenção:** "passivo" não significa necessariamente "não conduz eletricidade". A classificação é sobre a função do componente na infraestrutura de rede.

---

# 16. Exemplo de uma rede real

Imagine uma empresa:

```text
                 INTERNET
                    │
                    ▼
                ROTEADOR
                    │
                 FIREWALL
                    │
                    ▼
                 SWITCH
              ┌─────┼─────┐
              │     │     │
             PC    PC    AP
                          │
                       📱 💻
```

Agora adicionando a infraestrutura física:

```text
PC
 │
 │ Cabo de rede
 ▼
Patch Panel
 │
 │ Patch Cord
 ▼
Switch
 │
 ▼
Roteador
 │
 ▼
Internet
```

O **patch panel e os cabos** fazem parte da infraestrutura física.

O **switch e o roteador** participam ativamente da comunicação.

---

# 17. Relação com o que já estudamos

Você já estudou:

```text
Topologias
     ↓
Meios de transmissão
     ↓
UTP / STP
     ↓
Padrões T568A / T568B
     ↓
Equipamentos de rede
     ↓
Switch / Roteador / AP
     ↓
Comunicação na rede
```

Isso começa a montar uma visão muito mais completa de como uma rede realmente é construída.

---

# 🧠 O que realmente guardar

Não precisa decorar uma lista gigantesca.

Entenda principalmente:

```text
PASSIVO
→ infraestrutura física
→ organiza/conecta

ATIVO
→ participa ativamente da comunicação
→ possui eletrônica/processamento

SWITCH
→ conecta dispositivos na LAN
→ trabalha principalmente com MAC

ROTEADOR
→ conecta redes diferentes
→ trabalha com IP e roteamento

ACCESS POINT
→ fornece acesso Wi-Fi

PATCH PANEL
→ organiza/termina cabos

RACK
→ acomoda e organiza equipamentos
```

### Regra mental

> **Passivo = infraestrutura.**
>
> **Ativo = comunicação/processamento.**
