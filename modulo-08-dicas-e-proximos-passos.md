# Módulo 8 — Dicas, boas práticas e próximos passos

## Objetivos deste módulo
- Consolidar as melhores práticas aprendidas
- Evitar os erros mais comuns
- Descobrir recursos avançados para continuar evoluindo
- Montar um plano de prática pessoal

---

## As 10 melhores práticas

### 1. Sempre trabalhe em uma pasta dedicada

Crie uma pasta específica para cada projeto ou tarefa. O Claude trabalha dentro do contexto da pasta onde foi iniciado.

```
mkdir projeto-relatorios-2024
cd projeto-relatorios-2024
claude
```

### 2. Faça backups antes de operações em massa

Antes de rodar qualquer script que modifica muitos arquivos:

```
> Antes de executar, faça uma cópia da pasta atual como backup.
  Só então execute a operação.
```

### 3. Peça prévia antes de grandes mudanças

```
> Me mostre O QUE você faria, passo a passo, antes de executar qualquer coisa.
```

### 4. Seja específico nos pedidos

Quanto mais detalhes você fornecer, melhor o resultado:
- ❌ "Organiza isso"
- ✅ "Organize os arquivos .pdf por ano (extraindo do nome do arquivo), criando pastas no formato YYYY"

### 5. Use iterações pequenas

Não peça tudo de uma vez. Vá passo a passo:

```
> Vamos fazer isso em etapas. Primeiro, só leia os arquivos e me diga o que encontrou.
  Não faça nenhuma modificação ainda.
```

### 6. Releia o plano do Claude antes de aprovar

Quando o Claude mostra o que vai fazer, leia com atenção. Se algo parecer errado, cancele e reformule o pedido.

### 7. Não compartilhe arquivos sensíveis desnecessariamente

Se sua pasta tem arquivos com senhas, dados pessoais ou informações confidenciais, certifique-se de que o Claude precisa realmente acessá-los para a tarefa.

### 8. Peça explicações sempre que não entender

```
> Você usou o termo "regex" — pode me explicar em termos simples o que é?
```

### 9. Aproveite a memória da sessão

Você não precisa repetir contexto dentro da mesma sessão. Referencie o que foi feito:

```
> Com base no script que você criou antes, adicione agora um tratamento de erros.
```

### 10. Documente o que funciona

Quando encontrar um pedido que gerou exatamente o que precisava, salve-o em um arquivo de "receitas":

```
> Salve este prompt que funcionou bem em um arquivo chamado "receitas-claude.txt"
  para eu usar de referência no futuro.
```

---

## Erros comuns a evitar

| Erro | Por que é problema | Como evitar |
|------|-------------------|-------------|
| Pedir ao Claude para agir na pasta errada | Pode modificar arquivos do projeto errado | Sempre verifique em qual pasta está antes de iniciar |
| Aprovar sem ler o plano | Pode executar algo inesperado | Leia sempre o que o Claude vai fazer |
| Usar em arquivos únicos sem backup | Se der errado, não tem como voltar | Faça cópia antes |
| Pedidos muito vagos | Resultados genéricos ou errados | Seja específico sobre entrada e saída esperada |
| Confiar cegamente em scripts não testados | Scripts podem ter bugs | Teste sempre em dados fictícios primeiro |

---

## Recursos avançados para explorar depois

Quando você estiver confortável com o básico, explore:

### Modo não-interativo (automatização total)
```bash
claude -p "Consolide os CSVs desta pasta e gere um relatório" --no-interactive
```
Útil para rodar o Claude Code em scripts agendados.

### Integrações com IDE
O Claude Code funciona como extensão no VS Code e JetBrains — você pode usar dentro do editor de código.

### CLAUDE.md — Instruções permanentes
Crie um arquivo `CLAUDE.md` na pasta do projeto com instruções que o Claude sempre vai seguir:

```markdown
# Instruções para este projeto

- Sempre fazer backup antes de modificar arquivos
- Usar datas no formato DD/MM/YYYY
- Relatórios devem ser em português
- Nunca modificar arquivos na pasta /arquivos-originais
```

### Atalhos de teclado úteis
- `Ctrl + C` — interrompe a execução atual
- `↑` (seta pra cima) — repete o último comando
- `/compact` — quando a conversa ficar muito longa, comprime sem perder contexto

---

## Casos de uso para expandir seu repertório

Agora que você domina o básico, tente estes desafios:

**Nível 1 — Iniciante:**
- [ ] Criar um diário digital que organiza entradas por data
- [ ] Script para checar se todos os links em um arquivo funcionam
- [ ] Gerador de senhas aleatórias seguras salvas em arquivo

**Nível 2 — Intermediário:**
- [ ] Sistema de controle de estoque em CSV
- [ ] Script que baixa e organiza anexos de e-mail
- [ ] Conversor de formato de datas em planilhas

**Nível 3 — Avançado:**
- [ ] Dashboard simples em HTML gerado a partir de dados CSV
- [ ] Bot que monitora uma pasta e processa arquivos automaticamente
- [ ] API simples para consultar dados de uma planilha

---

## Seu plano de 30 dias

### Semana 1 — Consolidação
- Refaça todos os exercícios dos módulos anteriores sem olhar o gabarito
- Resolva 1 tarefa real do seu trabalho usando o Claude Code

### Semana 2 — Expansão
- Automatize uma tarefa que você faz toda semana
- Explore o modo `CLAUDE.md` para seu projeto principal

### Semana 3 — Desafios
- Complete pelo menos 3 desafios do Nível 1 acima
- Tente um do Nível 2

### Semana 4 — Integração
- Crie um "kit de ferramentas" pessoal: um conjunto de scripts que resolvem seus problemas mais comuns
- Documente tudo em um README claro

---

## Onde continuar aprendendo

- **Documentação oficial:** docs.anthropic.com/claude-code
- **GitHub do Claude Code:** github.com/anthropics/claude-code (exemplos e issues)
- **Comunidade:** Fóruns da Anthropic e comunidades no Reddit (r/ClaudeAI)

---

## Parabéns!

Você completou o curso introdutório de Claude Code. 

Você agora sabe:
- ✅ O que é o Claude Code e como ele se diferencia do Claude no chat
- ✅ Como instalar e configurar
- ✅ Como trabalhar com arquivos e pastas
- ✅ Como pedir scripts sem saber programar
- ✅ Como entender projetos existentes
- ✅ Como automatizar tarefas repetitivas
- ✅ Boas práticas de uso seguro

O Claude Code é uma ferramenta que cresce com você. Quanto mais você usa, mais percebe novas possibilidades. Comece pequeno, com tarefas reais do seu dia a dia, e expanda conforme ganhar confiança.

**Boa jornada!**

---

*Curso criado com Claude Code — Abril de 2026*
