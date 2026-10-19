# 🔎 Google Hacking (Google Dorking)

## 1. O que é Google Hacking?

**Google Hacking**, também conhecido como **Google Dorking**, é uma técnica de pesquisa avançada que utiliza operadores de busca para localizar informações específicas na Internet.

Esses operadores permitem filtrar resultados e encontrar páginas, documentos, diretórios e outros conteúdos que seriam mais difíceis de localizar por uma pesquisa comum.

Na segurança da informação, a técnica pode ser utilizada para identificar informações expostas publicamente e ajudar a avaliar a segurança de sites e sistemas.

**Importante:** Google Hacking não significa invadir o Google. O nome se refere ao uso avançado do mecanismo de busca.

---

## 2. Como funciona?

O Google rastreia páginas disponíveis na Web e pode armazenar informações sobre elas em seu índice.

Quando fazemos uma pesquisa, o mecanismo tenta encontrar resultados relevantes para os termos e operadores utilizados.

No Google Hacking, combinamos operadores para restringir os resultados.

Exemplo de pesquisa comum:

```text
redes de computadores
```

Pesquisa mais específica:

```text
"redes de computadores" filetype:pdf
```

A segunda pesquisa procura a expressão exata em conjunto com o filtro de arquivos PDF.

**Atenção:** um resultado aparecer no Google não significa necessariamente que o arquivo esteja acessível, atualizado ou vulnerável.

---

# 3. Principais operadores de pesquisa

## 3.1. `site:`

Permite restringir os resultados a um site ou domínio.

### Exemplo

```text
site:gov.br segurança da informação
```

**O que faz:** procura resultados relacionados à segurança da informação dentro do domínio `gov.br`.

Outro exemplo:

```text
site:edu.br redes de computadores
```

Pode ajudar a localizar materiais educacionais publicados em domínios `.edu.br`.

### Quando utilizar?

- Pesquisar informações dentro de um domínio.
- Encontrar páginas de uma organização.
- Fazer inventário de conteúdos públicos de um site autorizado.
- Restringir pesquisas a uma fonte específica.

---

## 3.2. `filetype:`

Permite restringir os resultados a um tipo de arquivo.

### Exemplos

```text
segurança da informação filetype:pdf
```

Procura documentos PDF relacionados ao assunto.

```text
redes de computadores filetype:pptx
```

Procura apresentações PowerPoint.

```text
programação Java filetype:docx
```

Procura documentos Word.

### Tipos de arquivo comuns

| Extensão | Tipo |
|---|---|
| `pdf` | Documento PDF |
| `docx` | Documento Word |
| `xlsx` | Planilha Excel |
| `pptx` | Apresentação PowerPoint |
| `txt` | Arquivo de texto |
| `csv` | Dados separados por delimitadores |
| `xml` | Documento estruturado em XML |
| `json` | Dados estruturados em JSON |

**Importante:** `filetype:` filtra os resultados por tipo de arquivo; não garante que todos os arquivos desse tipo sejam encontrados.

---

## 3.3. Aspas `" "`

As aspas são usadas para procurar uma expressão exata ou muito próxima dela.

### Exemplo

```text
"modelo OSI"
```

A pesquisa prioriza páginas que contenham essa expressão.

Outro exemplo:

```text
"segurança da informação" site:gov.br
```

Combina a expressão entre aspas com a restrição de domínio.

### Para que serve?

- Encontrar frases específicas.
- Localizar títulos.
- Pesquisar mensagens de erro.
- Procurar trechos conhecidos de documentação.

---

## 3.4. `-` — excluir termos

O sinal de menos permite excluir determinados termos dos resultados.

### Exemplo

```text
Java programação -curso
```

Procura informações sobre programação Java, excluindo resultados associados ao termo `curso`.

Outro exemplo:

```text
redes de computadores -jogos
```

Ajuda a excluir resultados relacionados a jogos.

O sinal deve ser colocado imediatamente antes do termo que se deseja excluir.

---

## 3.5. `OR` — uma opção ou outra

Permite pesquisar páginas relacionadas a um termo ou a outro.

### Exemplo

```text
Java OR Python programação
```

Procura resultados relacionados a Java ou Python e à programação.

O uso de parênteses pode ajudar a organizar consultas mais complexas, embora o comportamento exato dependa de como o mecanismo interpreta a pesquisa.

---

## 3.6. `intitle:`

Restringe a pesquisa a páginas cujo título contenha determinado termo.

### Exemplo

```text
intitle:segurança redes
```

Procura páginas com `segurança` no título, relacionadas a redes.

### Utilidade

Pode ajudar a localizar:

- Artigos.
- Tutoriais.
- Documentação.
- Páginas com títulos específicos.

---

## 3.7. `inurl:`

Procura páginas cujo endereço contenha determinado termo.

### Exemplo

```text
inurl:documentacao Java
```

Procura páginas com `documentacao` no endereço e relacionadas a Java.

### Utilidade

Pode ajudar a encontrar páginas de documentação, seções de um site ou recursos com caminhos específicos.

O operador não verifica se uma página é segura ou vulnerável.

---

## 3.8. `intext:`

Procura páginas cujo conteúdo textual contenha um termo.

### Exemplo

```text
intext:firewall redes
```

Procura páginas com o termo `firewall` no texto, relacionadas a redes.

---

## 3.9. `before:` e `after:`

Podem ser utilizados para restringir pesquisas por datas.

### Exemplos

```text
segurança da informação after:2025-01-01
```

Procura conteúdos associados a datas posteriores ao limite informado.

```text
redes de computadores before:2025-01-01
```

Procura conteúdos anteriores ao limite informado.

Esses filtros dependem das datas que o Google consegue identificar e não garantem uma data exata de publicação.

---

# 4. O que significa `index of/`?

Uma das expressões mais conhecidas em Google Hacking é:

```text
index of/
```

Ela está associada a páginas de listagem de diretórios.

## 4.1. O que é uma listagem de diretório?

Em alguns servidores Web, quando um diretório não possui uma página inicial configurada e a listagem de arquivos está habilitada, o servidor pode apresentar uma página com os arquivos e subdiretórios daquele local.

Uma listagem ilustrativa poderia mostrar:

```text
Index of /documentos/

Nome                 Tamanho
relatorio.pdf        250 KB
manual.txt           12 KB
imagens/             -
```

Isso é apenas um exemplo fictício.

## 4.2. Por que isso pode ser um problema?

Uma listagem pública pode revelar informações que o responsável pelo sistema não pretendia divulgar, como:

- Nomes de arquivos internos.
- Estrutura de diretórios.
- Documentos que deveriam ser privados.
- Arquivos de backup.
- Versões antigas de documentos.
- Informações sobre tecnologias utilizadas.

A gravidade depende do conteúdo exposto e das permissões aplicadas.

**A existência de `Index of` não significa automaticamente que existe uma vulnerabilidade grave.** Um diretório pode ser público por decisão legítima do responsável.

## 4.3. Como se proteger?

Quem administra o servidor deve:

- Desabilitar listagens de diretório quando não forem necessárias.
- Configurar permissões adequadas.
- Evitar armazenar arquivos privados em diretórios públicos.
- Remover arquivos antigos e backups desnecessários.
- Exigir autenticação para conteúdos restritos.
- Revisar o que pode ser acessado pela Web.

---

# 5. O que são operadores combinados?

É possível combinar operadores em uma mesma pesquisa para torná-la mais específica.

### Exemplo educacional

```text
site:gov.br "segurança da informação" filetype:pdf
```

Interpretação:

- `site:gov.br` restringe os resultados ao domínio.
- `"segurança da informação"` procura a expressão.
- `filetype:pdf` restringe os resultados a PDFs.

Outro exemplo:

```text
site:edu.br intitle:redes filetype:pdf
```

Interpretação:

- Procura dentro de `edu.br`.
- Prioriza páginas com `redes` no título.
- Filtra resultados em PDF.

### Ideia principal

Quanto mais critérios relevantes forem adicionados, mais específica pode ficar a pesquisa. Entretanto, critérios demais também podem excluir resultados úteis.

---

# 6. Google Hacking na segurança da informação

O Google Dorking pode ser utilizado em atividades de reconhecimento e auditoria de segurança.

## 6.1. Reconhecimento

Reconhecimento é a etapa de reunir informações sobre um alvo antes de uma avaliação de segurança.

Em um trabalho autorizado, pode envolver:

- Identificar páginas públicas.
- Localizar documentação publicada.
- Reconhecer tecnologias divulgadas publicamente.
- Verificar se informações institucionais estão expostas.
- Identificar possíveis divulgações acidentais.

## 6.2. Exposição de informações

Um problema ocorre quando informações que deveriam ser restritas ficam acessíveis publicamente.

Exemplos de categorias de risco:

- Backups publicados.
- Arquivos de configuração expostos.
- Documentos internos publicados por engano.
- Listagens de diretório desnecessárias.
- Mensagens de erro que revelam detalhes internos.

Essas categorias descrevem riscos que devem ser investigados em sistemas autorizados; não significam que o Google consiga localizar todos esses conteúdos.

## 6.3. O que o Google Dorking não faz?

Por si só, o Google Dorking não:

- Quebra senhas.
- Invade automaticamente um servidor.
- Contorna autenticação.
- Garante acesso a arquivos privados.
- Confirma que um sistema possui vulnerabilidade explorável.

É uma técnica de pesquisa e descoberta de informações. Qualquer investigação adicional precisa ser feita com autorização e dentro do escopo permitido.

---

# 7. Diferença entre informação pública e informação sensível

Nem toda informação pública representa um problema de segurança.

| Tipo de informação | Exemplo | Avaliação |
|---|---|---|
| Pública e intencional | Manual de usuário publicado oficialmente | Normalmente esperado |
| Técnica pública | Documentação de uma API pública | Depende do contexto |
| Exposta por engano | Backup de um sistema publicado sem intenção | Pode representar risco |
| Confidencial | Senhas, tokens ou dados pessoais de terceiros | Não deve ser acessada ou utilizada sem autorização |

Uma informação estar indexada não significa que exista autorização para utilizá-la de qualquer maneira.

Se encontrar dados sensíveis de terceiros, não os baixe, compartilhe ou tente utilizar. Registre apenas o mínimo necessário e comunique o responsável pelo sistema por um canal apropriado.

---

# 8. Laboratório seguro para praticar

É possível aprender os operadores sem procurar informações privadas de terceiros.

## Exercício 1 — localizar material de estudo

```text
redes de computadores filetype:pdf
```

Objetivo: observar como o tipo de arquivo altera os resultados.

## Exercício 2 — pesquisar em um domínio específico

```text
site:gov.br segurança digital
```

Objetivo: restringir os resultados a um domínio.

## Exercício 3 — combinar operadores

```text
site:edu.br "modelo OSI" filetype:pdf
```

Objetivo: combinar domínio, expressão exata e tipo de arquivo.

## Exercício 4 — localizar títulos

```text
intitle:documentação Java
```

Objetivo: observar como a busca pelo título afeta os resultados.

## Exercício 5 — excluir um termo

```text
redes de computadores -jogos
```

Objetivo: comparar os resultados com e sem o termo excluído.

## Exercício 6 — compreender listagens de diretórios

Estude uma listagem fictícia ou um ambiente de laboratório criado para esse propósito.

Identifique quais informações poderiam ser reveladas e quais configurações impediriam a exposição.

**Não utilize buscas direcionadas para encontrar senhas, tokens, documentos privados ou painéis de terceiros.** Se a atividade for uma auditoria real, utilize apenas os domínios e sistemas explicitamente autorizados.

---

# 9. Como corrigir uma exposição em um site próprio

Se você administra um site e descobre que arquivos aparecem nos resultados de busca:

1. Verifique se o arquivo deveria ser público.
2. Restrinja o acesso no servidor ou remova o arquivo do diretório público.
3. Revogue e substitua credenciais ou tokens expostos.
4. Investigue logs e possíveis acessos indevidos.
5. Solicite a remoção do resultado pelos canais apropriados do mecanismo de busca, quando aplicável.
6. Confirme que o conteúdo não continua acessível diretamente pela URL.

**Importante:** remover uma página dos resultados de busca não protege um arquivo que continua publicamente acessível. É necessário corrigir a origem da exposição.

---

# 10. Relação com redes e desenvolvimento

O Google Hacking se conecta a outros assuntos estudados em redes e segurança:

- **DNS:** ajuda a entender como nomes de domínio são associados a endereços IP.
- **HTTP/HTTPS:** explica como navegadores e servidores trocam informações.
- **Servidores Web:** ajudam a entender como páginas e arquivos são disponibilizados.
- **Permissões:** determinam quem pode acessar determinados recursos.
- **Autenticação:** controla quem pode entrar em uma área restrita.
- **Configuração de servidores:** influencia a exposição de diretórios e arquivos.
- **Segurança de aplicações:** busca evitar divulgação de dados e configurações sensíveis.

Para quem pretende desenvolver aplicações, a principal lição é que **um sistema não deve depender do fato de uma URL ser difícil de encontrar para manter seus dados protegidos**.

Arquivos confidenciais precisam de controles de acesso reais.

---

# 11. Erros comuns ao estudar Google Hacking

- Acreditar que todo resultado encontrado representa uma vulnerabilidade.
- Confundir indexação com autorização.
- Pensar que `filetype:` encontra absolutamente todos os arquivos.
- Acreditar que `index of/` sempre revela dados confidenciais.
- Imaginar que uma busca consegue invadir um servidor automaticamente.
- Acessar ou baixar informações privadas durante uma prática.
- Confundir remoção dos resultados do Google com correção da exposição no servidor.

---

# 12. Resumo para revisão rápida

| Operador ou conceito | Função |
|---|---|
| Google Hacking / Dorking | Pesquisa avançada aplicada também ao reconhecimento de segurança |
| `site:` | Restringe os resultados a um domínio ou site |
| `filetype:` | Filtra por tipo de arquivo |
| `"frase"` | Procura uma expressão exata |
| `-termo` | Exclui um termo |
| `OR` | Combina alternativas |
| `intitle:` | Pesquisa um termo no título |
| `inurl:` | Pesquisa um termo no endereço |
| `intext:` | Pesquisa um termo no texto |
| `before:` | Filtra por data anterior |
| `after:` | Filtra por data posterior |
| `index of/` | Expressão associada a listagens de diretórios |
| Reconhecimento | Coleta de informações sobre um alvo |
| Exposição de dados | Disponibilização indevida de informações |
| Remediação | Correção do problema identificado |

---

# 13. Perguntas para revisar o conteúdo

Tente responder sem consultar as anotações:

1. O que é Google Hacking?
2. Qual é a diferença entre Google Hacking e invasão de um sistema?
3. Para que serve o operador `site:`?
4. Qual é a função de `filetype:`?
5. Para que servem as aspas em uma pesquisa?
6. Como o sinal `-` altera os resultados?
7. Qual é a diferença entre `intitle:` e `inurl:`?
8. O que é uma listagem de diretório?
9. Por que uma listagem de diretório pode representar um risco?
10. Uma página aparecer no Google significa que ela é vulnerável? Por quê?
11. Qual é a diferença entre informação pública e informação confidencial exposta?
12. Como um administrador pode corrigir uma exposição de arquivos?
13. Por que remover um resultado do Google não é suficiente se o arquivo continua acessível?
14. Como o Google Dorking pode ser usado em uma auditoria autorizada?
15. Por que uma aplicação não deve depender de URLs difíceis de adivinhar para proteger informações?

---

# 14. Conclusão

O Google Hacking utiliza operadores de pesquisa para localizar informações específicas que já estão disponíveis ou indexadas na Web.

É uma ferramenta útil para pesquisa, reconhecimento e auditoria de segurança, mas os resultados precisam ser interpretados com cuidado.

Os conceitos mais importantes para guardar são:

- `site:` restringe por domínio.
- `filetype:` restringe por tipo de arquivo.
- Aspas ajudam a pesquisar expressões exatas.
- `index of/` está associado à listagem de diretórios.
- Operadores podem ser combinados.
- Um resultado encontrado não confirma, por si só, uma vulnerabilidade.
- A prática deve respeitar autorização, privacidade e escopo.
- A proteção real de arquivos depende de configuração e controles de acesso adequados.

**Mentalidade de segurança:** descobrir uma exposição é apenas uma etapa. Entender o risco, corrigir a causa e verificar a correção é o que transforma a descoberta em trabalho de segurança da informação.

---

## Referências

- [Ajuda oficial da Pesquisa Google — Refinar pesquisas](https://support.google.com/websearch/answer/2466433?hl=pt-br)
- [OWASP Web Security Testing Guide — Search Engine Discovery and Reconnaissance](https://owasp.org/www-project-web-security-testing-guide/)

Use estas referências para conferir os operadores e aprofundar o estudo sobre reconhecimento e exposição de informações.
