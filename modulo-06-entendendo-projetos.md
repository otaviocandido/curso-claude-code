# Módulo 6 — Entendendo projetos existentes

## Objetivos deste módulo
- Pedir ao Claude para explicar um projeto ou código que você recebeu
- Descobrir o que um programa faz sem saber programar
- Encontrar informações específicas dentro de projetos grandes
- Fazer perguntas sobre código de forma eficiente

---

## O cenário comum

Você herdou um projeto, recebeu arquivos de um fornecedor, ou encontrou um script online. Você não sabe o que faz. Com o Claude Code:

```
> Tenho essa pasta com vários arquivos que recebi de um freelancer. 
  Pode me dar uma visão geral de o que esse projeto faz, 
  em linguagem simples?
```

O Claude vai analisar os arquivos e te dar um resumo em português claro.

---

## Comandos úteis para explorar projetos

### Visão geral do projeto

```
> Me dê uma visão geral desta pasta: quantos arquivos existem, 
  que tipos são, e qual parece ser o propósito do projeto?
```

### Entender um arquivo específico

```
> O que o arquivo main.py faz? Explique como se eu tivesse 10 anos.
```

### Encontrar onde algo está

```
> Onde neste projeto é definido o preço dos produtos?
```

```
> Em qual arquivo está a lógica que envia e-mails?
```

### Mapear dependências

```
> Este projeto depende de quais outros sistemas ou serviços externos?
```

---

## Situações práticas

### Situação 1: Site que parou de funcionar

```
> Este site estava funcionando e parou. Os arquivos estão nesta pasta.
  Pode identificar o que pode ter causado o problema?
```

### Situação 2: Entender uma fórmula ou cálculo

```
> No arquivo calculos.py, tem uma função chamada calcular_desconto.
  Me explique como ela calcula o desconto, com um exemplo numérico.
```

### Situação 3: Verificar segurança básica

```
> Alguém me mandou esse script para instalar no meu servidor.
  Pode verificar se tem algo suspeito ou perigoso nele?
```

### Situação 4: Adaptar código para seu caso

```
> Esse script foi criado para Windows mas preciso que funcione no Mac também.
  O que precisa mudar?
```

---

## Fazendo perguntas em série

Você pode ir aprofundando:

```
> O que esse projeto faz?
```
*(Claude explica em alto nível)*

```
> Interessante. Me explica mais sobre a parte de autenticação que você mencionou.
```
*(Claude detalha)*

```
> E essa parte usa alguma informação sensível como senhas? Onde elas ficam armazenadas?
```
*(Claude aponta os pontos relevantes)*

---

## Gerando documentação automática

Se você precisa documentar um projeto que recebeu:

```
> Leia todos os arquivos deste projeto e gere um arquivo DOCUMENTACAO.md
  explicando:
  - Para que serve o projeto
  - Como instalar e rodar
  - O que cada arquivo principal faz
  - Quais configurações podem ser ajustadas
  
  Escreva de forma que alguém não técnico consiga entender.
```

---

## Comparando versões

Se você tem duas versões de um arquivo e quer saber o que mudou:

```
> Tenho dois arquivos: app-v1.py e app-v2.py.
  Quais são as diferenças entre eles? O que foi adicionado, 
  removido ou modificado?
```

---

## Projeto prático do módulo

**Analisar um projeto de exemplo:**

Primeiro, vamos criar um projeto fictício para analisar:

```
> Crie uma pasta chamada "projeto-exemplo" com os seguintes arquivos 
  simulando um sistema simples de cadastro de clientes:
  - main.py (arquivo principal)
  - banco.py (simulação de banco de dados)  
  - relatorios.py (geração de relatórios)
  - config.txt (configurações)
  - README.md (documentação básica)
  
  Cada arquivo deve ter código Python real, mas simples.
```

Agora pratique analisar:

```
> Entre na pasta projeto-exemplo. Analise todos os arquivos e me 
  explique como esse sistema funciona, como se você fosse apresentar 
  para alguém que vai usar o sistema mas não programa.
```

```
> Nesse projeto, como eu adicionaria um novo cliente? 
  Quais arquivos precisariam ser modificados?
```

---

## Checklist

- [ ] Pedi ao Claude uma visão geral de uma pasta/projeto
- [ ] Pedi explicação de um arquivo específico
- [ ] Gerei documentação automática de um projeto
- [ ] Completei o projeto prático de análise

**Próximo módulo →** [Módulo 7: Automatizando tarefas do dia a dia](modulo-07-automatizando-tarefas.md)
