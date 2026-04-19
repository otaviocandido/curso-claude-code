# Módulo 5 — Pedindo ao Claude para escrever e editar código

## Objetivos deste módulo
- Pedir scripts úteis sem saber programar
- Entender o que o Claude criou (sem precisar decorar nada)
- Rodar scripts simples
- Corrigir erros com a ajuda do Claude

---

## Você não precisa saber programar para isso

Uma das melhores coisas do Claude Code é que você pode pedir programas em linguagem natural e ele cria o código por você. Você apenas:

1. Descreve o que quer que o programa faça
2. Claude escreve o código
3. Claude executa (com sua aprovação)
4. Você vê o resultado

---

## Qual linguagem o Claude vai usar?

O Claude escolhe automaticamente a melhor linguagem para a tarefa. As mais comuns:

- **Python** — para processar dados, automatizar tarefas, trabalhar com arquivos
- **JavaScript/Node.js** — para coisas relacionadas à web
- **Bash/Shell** — para tarefas rápidas no terminal

Para a maioria das tarefas de leigos, o Claude usará **Python** — e o mais importante: você não precisa entender o código, apenas o resultado.

> **Nota:** Python precisa estar instalado. Se o Claude pedir para instalar, siga as instruções em python.org

---

## Exemplos práticos: scripts úteis do dia a dia

### 1. Renomear arquivos em massa

```
> Tenho uma pasta com fotos nomeadas de forma aleatória (IMG_4832.jpg, etc).
  Escreva um script que renomeie todas as fotos .jpg para o formato 
  "foto_001.jpg", "foto_002.jpg", etc, em ordem alfabética.
```

### 2. Converter PDF para texto

```
> Escreva um script Python que leia todos os arquivos .pdf nesta pasta
  e salve o texto de cada um em um arquivo .txt com o mesmo nome
```

### 3. Organizar downloads por data

```
> Crie um script que pegue todos os arquivos da pasta Downloads,
  verifique a data de criação de cada um, e os mova para subpastas
  no formato "2024/Janeiro", "2024/Fevereiro", etc.
```

### 4. Gerar relatório de uma planilha

```
> Tenho um arquivo vendas.csv com colunas: produto, quantidade, preco_unitario, data.
  Crie um script que leia esse CSV e gere um arquivo PDF com:
  - Total de vendas por produto
  - Total geral do mês
  - Produto mais vendido
  - Gráfico de vendas por dia
```

### 5. Enviar resumo por e-mail (com sua configuração)

```
> Crie um script que leia o arquivo relatorio.txt e envie um e-mail 
  com o resumo para contato@empresa.com usando meu Gmail.
  Me pergunte as credenciais de forma segura.
```

---

## Entendendo o que o Claude criou

Você não precisa entender cada linha, mas é útil saber pedir uma explicação:

```
> Você criou esse script. Pode me explicar em linguagem simples 
  o que cada parte faz? Sem termos técnicos.
```

O Claude vai explicar como se você tivesse 12 anos:
```
Claude: "Esse script faz o seguinte:
  1. Abre a pasta que você indicou
  2. Procura todos os arquivos que terminam em .jpg
  3. Para cada arquivo encontrado, cria um novo nome no formato foto_001
  4. Renomeia o arquivo
  5. No final, mostra quantos arquivos foram renomeados"
```

---

## Quando o código der erro

Erros acontecem — é normal. Mas com o Claude, corrigir é fácil:

```
> O script que você criou deu o seguinte erro:
  "FileNotFoundError: No such file or directory: 'pasta-fotos'"
  Pode consertar?
```

O Claude vai diagnosticar e corrigir automaticamente. Você não precisa entender o erro.

---

## Testando antes de usar em arquivos importantes

Sempre teste em cópias:

```
> Antes de rodar em meus arquivos reais, crie uma pasta de teste 
  com arquivos fictícios e rode o script lá primeiro para eu ver o resultado
```

---

## Modificando scripts existentes

Se você tem um script que quase funciona, mas não exatamente:

```
> Esse script renomeia os arquivos, mas quero que ele também 
  crie um log.txt registrando cada renomeação feita. Pode adicionar isso?
```

---

## Projeto prático do módulo

**Criar um organizador automático de arquivos:**

```
> Vamos criar um script Python chamado "organizador.py" que:
  1. Peça ao usuário que informe uma pasta
  2. Liste todos os arquivos nela
  3. Organize em subpastas por extensão:
     - Imagens (.jpg, .png, .gif) → pasta "Imagens"
     - Documentos (.pdf, .docx, .txt) → pasta "Documentos"  
     - Planilhas (.xlsx, .csv) → pasta "Planilhas"
     - Outros → pasta "Outros"
  4. Mostre um resumo de quantos arquivos foram movidos para cada pasta
  
  Primeiro me mostre o código, depois me explique cada parte, 
  e então pergunte se eu quero executar.
```

---

## Checklist

- [ ] Pedi ao Claude para criar um script simples
- [ ] Pedi uma explicação do código criado
- [ ] Entendi como reportar erros para o Claude corrigir
- [ ] Completei o projeto do organizador de arquivos

**Próximo módulo →** [Módulo 6: Entendendo projetos existentes](modulo-06-entendendo-projetos.md)
