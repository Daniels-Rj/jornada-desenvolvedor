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

## 3
