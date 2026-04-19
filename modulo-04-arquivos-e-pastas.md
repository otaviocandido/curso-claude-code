# Módulo 4 — Trabalhando com arquivos e pastas

## Objetivos deste módulo
- Pedir ao Claude para ler, criar, editar e organizar arquivos
- Trabalhar com diferentes tipos de arquivo (txt, csv, json, pdf)
- Organizar pastas automaticamente
- Fazer buscas dentro de arquivos

---

## O que o Claude pode fazer com arquivos

O Claude Code é excelente em manipulação de arquivos. Aqui está o que você pode pedir:

| Ação | Exemplo de pedido |
|------|------------------|
| Criar | "Crie um arquivo lista-compras.txt" |
| Ler | "Leia o arquivo e me explique o conteúdo" |
| Editar | "No arquivo, mude 'João' para 'Maria' em todos os lugares" |
| Renomear | "Renomeie esse arquivo para relatorio-final.txt" |
| Mover | "Mova este arquivo para a pasta 'arquivos-antigos'" |
| Copiar | "Faça uma cópia deste arquivo chamada backup.txt" |
| Buscar | "Encontre todos os arquivos que contêm a palavra 'urgente'" |
| Organizar | "Organize esses arquivos por tipo numa estrutura de pastas" |

---

## Trabalhando com arquivos de texto (.txt, .md)

O caso mais simples. O Claude lê e escreve texto puro.

**Criar um arquivo de anotações:**
```
> Crie um arquivo chamado reuniao-2024-01-15.txt com uma ata de reunião 
  fictícia para uma equipe de marketing discutindo o lançamento de um produto
```

**Extrair informações:**
```
> Leia o arquivo reuniao-2024-01-15.txt e me liste:
  - Quem participou
  - Quais decisões foram tomadas
  - Quais são os próximos passos
```

---

## Trabalhando com CSV (planilhas simples)

CSV é um formato de planilha que o Claude lê muito bem.

**Exemplo — criando dados fictícios para praticar:**
```
> Crie um arquivo clientes.csv com 10 clientes fictícios contendo as colunas:
  nome, email, cidade, data_cadastro, valor_total_compras
```

**Analisando o CSV:**
```
> Leia o arquivo clientes.csv e me diga:
  - Quantos clientes são de São Paulo?
  - Qual o valor médio de compras?
  - Quem é o cliente com maior valor total?
```

**Modificando o CSV:**
```
> No arquivo clientes.csv, adicione uma coluna "categoria" com os valores:
  - "VIP" para clientes com mais de R$5000 em compras
  - "Regular" para os demais
```

---

## Trabalhando com JSON

JSON é um formato de dados muito usado em sistemas. Parece complicado, mas o Claude simplifica tudo.

**Criando um JSON:**
```
> Crie um arquivo cardapio.json com um cardápio fictício de restaurante, 
  com categorias (entradas, pratos principais, sobremesas) e para cada item: 
  nome, descrição e preço
```

**Lendo e transformando:**
```
> Leia o arquivo cardapio.json e crie um arquivo cardapio.txt legível,
  formatado como um menu de restaurante bonito, com os preços em reais
```

---

## Organizando pastas automaticamente

Esta é uma das superpoderes do Claude Code — organizar bagunça de arquivos.

**Exemplo prático:**

Imagine uma pasta com 50 arquivos misturados. Peça:
```
> Analise os arquivos nesta pasta e proponha uma estrutura de organização 
  por tipo e data. Mostre a proposta antes de executar.
```

O Claude vai sugerir algo como:
```
/documentos
  /2023
  /2024
/imagens
/planilhas
/outros
```

Então você aprova e ele executa.

---

## Buscando dentro de arquivos

```
> Busque em todos os arquivos .txt desta pasta qualquer menção à palavra 
  "prazo" e me mostre quais arquivos contêm essa palavra e em qual contexto
```

```
> Encontre em qual arquivo desta pasta está o e-mail contato@empresa.com
```

---

## Projeto prático do módulo

Vamos simular uma situação real: organizar relatórios mensais.

**Passo 1 — Crie os arquivos de teste:**
```
> Crie 6 arquivos fictícios de relatório mensal, nomeados no formato 
  "relatorio-YYYY-MM.txt", de julho a dezembro de 2024. 
  Cada um deve ter um resumo de vendas fictício de 3 parágrafos.
```

**Passo 2 — Analise todos:**
```
> Leia todos os arquivos relatorio-*.txt e crie um resumo executivo 
  consolidado chamado "resumo-2024-semestre2.txt" comparando os 6 meses
```

**Passo 3 — Organize:**
```
> Mova todos os arquivos relatorio-*.txt para uma subpasta chamada 
  "relatorios-mensais" e mantenha o resumo na pasta principal
```

---

## Checklist

- [ ] Criei e li arquivos de texto
- [ ] Trabalhei com um arquivo CSV
- [ ] Entendi como usar JSON com o Claude
- [ ] Completei o projeto prático de organização de relatórios

**Próximo módulo →** [Módulo 5: Pedindo ao Claude para escrever código](modulo-05-escrevendo-codigo.md)
