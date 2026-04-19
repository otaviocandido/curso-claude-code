# Módulo 2 — Instalação passo a passo

## Objetivos deste módulo
- Instalar o Node.js (necessário para o Claude Code)
- Criar uma conta Anthropic e obter sua chave de API
- Instalar o Claude Code
- Fazer sua primeira verificação de funcionamento

---

## Passo 1: Instalar o Node.js

O Claude Code precisa do **Node.js** para funcionar. Node.js é uma tecnologia que permite rodar programas JavaScript no seu computador — você não precisa entender como funciona, só instalar.

### Como instalar:

1. Acesse **nodejs.org**
2. Clique no botão verde grande (versão LTS — a mais estável)
3. Baixe e instale normalmente (Next, Next, Finish)

### Verificar se instalou corretamente:

Abra o terminal e digite:
```
node --version
```

Se aparecer algo como `v20.11.0`, está funcionando!

---

## Passo 2: Criar conta na Anthropic

O Claude Code usa a API da Anthropic, que requer uma conta.

1. Acesse **console.anthropic.com**
2. Clique em "Sign Up"
3. Crie sua conta com e-mail
4. Confirme o e-mail

### Obter a chave de API:

1. Faça login no console.anthropic.com
2. No menu lateral, clique em **"API Keys"**
3. Clique em **"Create Key"**
4. Dê um nome (ex: "meu-claude-code")
5. **Copie a chave gerada** — ela começa com `sk-ant-...`

> **IMPORTANTE:** Trate sua chave de API como uma senha. Nunca compartilhe publicamente, não coloque em documentos acessíveis a outros.

### Sobre os custos:

O Claude Code usa créditos da API Anthropic. Você paga pelo uso (por tokens processados), não por assinatura mensal. Para uso leve (aprender, tarefas ocasionais), o custo é muito baixo — alguns centavos de dólar por sessão.

A Anthropic oferece créditos iniciais gratuitos para novos usuários.

---

## Passo 3: Instalar o Claude Code

Abra o terminal e execute este único comando:

```
npm install -g @anthropic-ai/claude-code
```

Aguarde a instalação terminar (pode demorar 1-2 minutos).

### Verificar a instalação:

```
claude --version
```

Deve aparecer o número da versão instalada.

---

## Passo 4: Configurar sua chave de API

Quando você rodar o Claude Code pela primeira vez, ele pedirá sua chave. Mas você pode configurar agora:

**Opção A — Configuração automática (recomendado):**

Simplesmente rode `claude` pela primeira vez e siga as instruções na tela. Ele vai te pedir a chave e salvar automaticamente.

**Opção B — Configuração manual:**

No terminal, execute:

```
# Mac/Linux
export ANTHROPIC_API_KEY="sua-chave-aqui"

# Windows (PowerShell)
$env:ANTHROPIC_API_KEY="sua-chave-aqui"
```

Para salvar permanentemente no Windows:
1. Abra "Variáveis de Ambiente do Sistema"
2. Crie nova variável: `ANTHROPIC_API_KEY` = sua chave

---

## Passo 5: Primeiro teste!

Crie uma pasta de teste e abra o Claude Code:

```
mkdir teste-claude
cd teste-claude
claude
```

Se tudo estiver certo, você verá a interface do Claude Code no terminal. Algo como:

```
╭──────────────────────────────────────╮
│  Claude Code  v1.x.x                 │
│  Pasta atual: /teste-claude          │
│                                      │
│  Digite sua mensagem ou /help        │
╰──────────────────────────────────────╯
>
```

### Seu primeiro comando:

```
> Olá! Pode criar um arquivo chamado ola.txt com a mensagem "Funcionou!"?
```

O Claude vai criar o arquivo. Verifique se ele apareceu:

```
ls
```

Deve mostrar `ola.txt`. Abra o arquivo para confirmar o conteúdo. **Parabéns — o Claude Code está funcionando!**

Para sair do Claude Code, digite:
```
/exit
```
Ou pressione `Ctrl + C`.

---

## Solução de problemas comuns

| Problema | Solução |
|----------|---------|
| `command not found: claude` | Feche e reabra o terminal após a instalação |
| `npm: command not found` | O Node.js não foi instalado corretamente — repita o Passo 1 |
| Erro de chave de API | Verifique se copiou a chave completa, sem espaços |
| Erro de permissão no Mac/Linux | Tente: `sudo npm install -g @anthropic-ai/claude-code` |

---

## Checklist

- [ ] Node.js instalado e verificado
- [ ] Conta Anthropic criada
- [ ] Chave de API obtida e configurada
- [ ] Claude Code instalado
- [ ] Primeiro arquivo criado com sucesso

**Próximo módulo →** [Módulo 3: Sua primeira sessão](modulo-03-primeira-sessao.md)
