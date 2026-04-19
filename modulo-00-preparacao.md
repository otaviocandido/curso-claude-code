# Módulo 0 — Preparação: O que você precisa antes de começar

## Objetivos deste módulo
- Entender o que é um terminal
- Saber navegar em pastas pelo terminal
- Estar pronto para instalar o Claude Code

---

## O que é um terminal?

O **terminal** (também chamado de "prompt de comando" ou "linha de comando") é um programa onde você digita instruções para o computador em vez de clicar em ícones.

Parece assustador? Não precisa ser. Pense nele como um chat — você digita um comando, o computador responde.

**Como abrir o terminal:**

| Sistema | Como abrir |
|---------|-----------|
| Windows | Pressione `Win + R`, digite `cmd` e Enter. Ou procure por "PowerShell" no menu Iniciar |
| Mac | Pressione `Cmd + Espaço`, digite "Terminal" e Enter |
| Linux | Pressione `Ctrl + Alt + T` |

---

## Comandos básicos que você vai usar

Você não precisa memorizar isso agora — apenas saiba que eles existem.

### Ver em qual pasta você está
```
pwd
```
*(no Windows: `cd`)*

### Listar arquivos na pasta atual
```
ls
```
*(no Windows: `dir`)*

### Entrar em uma pasta
```
cd nome-da-pasta
```

### Voltar uma pasta
```
cd ..
```

### Criar uma pasta nova
```
mkdir nome-da-pasta
```

---

## Exercício prático

1. Abra o terminal no seu computador
2. Digite `pwd` (Mac/Linux) ou `cd` (Windows) e pressione Enter
3. O terminal vai mostrar em qual pasta você está
4. Digite `ls` (Mac/Linux) ou `dir` (Windows) para ver os arquivos
5. Parabéns! Você usou o terminal!

---

## Conceito importante: o que é uma "pasta de projeto"?

Quando você usa o Claude Code, sempre trabalha dentro de uma **pasta**. Tudo que o Claude fizer — criar arquivos, ler código, fazer alterações — acontece dentro dessa pasta.

É como uma área de trabalho: você entra nela, e o Claude trabalha com o que está ali.

**Crie sua pasta de prática agora:**
```
mkdir minha-pasta-claude
cd minha-pasta-claude
```

Pronto! Você já está preparado para o próximo módulo.

---

## Checklist antes de continuar

- [ ] Consegui abrir o terminal
- [ ] Entendi o conceito de pasta/diretório
- [ ] Criei uma pasta chamada `minha-pasta-claude`

**Próximo módulo →** [Módulo 1: O que é o Claude Code](modulo-01-o-que-e-claude-code.md)
