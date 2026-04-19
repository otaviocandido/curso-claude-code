# Módulo 7 — Automatizando tarefas do dia a dia

## Objetivos deste módulo
- Identificar tarefas repetitivas que podem ser automatizadas
- Criar automações práticas para uso real
- Combinar múltiplos passos em um único comando
- Aprender a criar "receitas" reutilizáveis

---

## O princípio da automação

Se você faz algo mais de 3 vezes, o Claude pode automatizar. Pergunte-se:

> "Existe algo que faço toda semana que é repetitivo e chato?"

Exemplos típicos:
- Consolidar planilhas de vendas todo mês
- Renomear e organizar fotos de clientes
- Gerar relatórios em PDF a partir de dados
- Criar pastas com estrutura padrão para novos projetos
- Converter formatos de arquivo (PDF→TXT, DOCX→PDF)
- Fazer backup de arquivos importantes

---

## Automação 1: Gerador de estrutura de projeto

Toda vez que você inicia um projeto, precisa criar as mesmas pastas. Automatize:

```
> Crie um script chamado "novo-projeto.py" que:
  1. Pergunte o nome do projeto
  2. Crie uma pasta com esse nome
  3. Dentro, crie a estrutura:
     /documentos
     /imagens  
     /arquivos
     /backups
  4. Crie um arquivo README.txt com: nome do projeto e data de criação
  5. Mostre "Projeto [nome] criado com sucesso!"
```

Agora toda vez que quiser um novo projeto:
```
python novo-projeto.py
```

---

## Automação 2: Consolidador de planilhas

Você recebe 12 arquivos CSV (um por mês) e precisa juntar tudo:

```
> Crie um script "consolida-vendas.py" que:
  1. Leia todos os arquivos .csv nesta pasta
  2. Junte todos em uma única planilha
  3. Adicione uma coluna "mes" extraída do nome do arquivo
  4. Salve como "vendas-consolidadas.csv"
  5. Mostre um resumo: total de linhas, período coberto, total de vendas
```

---

## Automação 3: Relatório semanal automático

```
> Tenho um arquivo dados.csv que é atualizado toda semana.
  Crie um script "relatorio-semanal.py" que:
  1. Leia o dados.csv
  2. Calcule as principais métricas (total, média, top 5, comparação com semana anterior)
  3. Gere um arquivo "relatorio-[data-hoje].txt" formatado profissionalmente
  4. Mostre na tela um resumo do que foi gerado
```

---

## Automação 4: Backup organizado

```
> Crie um script "backup.py" que:
  1. Pergunte qual pasta fazer backup
  2. Crie uma cópia na pasta "Backups" com o nome: 
     "[pasta-original]_backup_[data-hora]"
  3. Mostre quantos arquivos foram copiados e o tamanho total
```

---

## Automação 5: Conversor em lote

```
> Tenho vários arquivos .docx que preciso converter para .pdf.
  Crie um script que converta todos os .docx desta pasta para .pdf
  e salve os PDFs em uma subpasta chamada "pdfs"
```

---

## Combinando automações

Você pode encadear várias tarefas em um único pedido:

```
> Faça o seguinte processo completo:
  1. Leia todos os arquivos .csv desta pasta
  2. Consolide em um único arquivo
  3. Gere um relatório de resumo em PDF
  4. Mova os CSVs originais para uma pasta "processados/[mes-atual]"
  5. Crie um log.txt registrando: data, quantos arquivos processados, total de registros
```

---

## Criando um menu de automações

Se você usa várias automações, crie um "painel":

```
> Crie um script "menu.py" que mostre um menu assim:

  === AUTOMAÇÕES ===
  1. Novo projeto
  2. Consolidar planilhas
  3. Gerar relatório semanal
  4. Fazer backup
  5. Sair
  
  E execute o script correspondente de acordo com a escolha do usuário.
```

---

## Projeto integrador do módulo

**Situação real:** Você é gestor de uma pequena equipe de vendas. Todo mês precisa:
- Receber os relatórios individuais de cada vendedor (arquivos CSV)
- Consolidar tudo
- Gerar um relatório com ranking de vendedores
- Arquivar os arquivos do mês anterior

```
> Vamos criar um sistema completo de gestão de relatórios de vendas.
  
  Passo 1: Crie arquivos CSV fictícios de 5 vendedores para janeiro e fevereiro de 2024,
  cada um com colunas: data, produto, quantidade, valor_unitario.
  
  Passo 2: Crie um script "fechamento-mensal.py" que:
  - Leia todos os CSVs da pasta atual
  - Calcule o total de vendas por vendedor
  - Gere um relatório "ranking-[mes].txt" com o ranking completo
  - Mova os CSVs processados para "historico/[mes]"
  - Registre tudo em um log
  
  Passo 3: Execute o script e mostre o resultado.
```

---

## Checklist

- [ ] Criei pelo menos 2 scripts de automação práticos
- [ ] Entendi como combinar múltiplos passos em um pedido
- [ ] Completei o projeto integrador de relatórios de vendas

**Próximo módulo →** [Módulo 8: Dicas, boas práticas e próximos passos](modulo-08-dicas-e-proximos-passos.md)
