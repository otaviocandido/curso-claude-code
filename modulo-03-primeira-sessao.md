# Módulo 3 — Sua primeira sessão: conversando com o Claude Code

## Objetivos deste módulo
- Entender a interface do Claude Code
- Aprender os comandos especiais (começam com `/`)
- Saber como fazer boas perguntas
- Entender como aprovar ou rejeitar ações

---

## A interface do Claude Code

Quando você digita `claude` no terminal dentro de uma pasta, você entra em uma **sessão interativa**. Pense nela como um chat no terminal.

```
> sua mensagem vai aqui
```

O `>` indica que o Claude está esperando você digitar.

---

## Os comandos especiais

Comandos que começam com `/` são instruções especiais para o Claude Code (não são mensagens enviadas à IA).

| Comando | O que faz |
|---------|-----------|
| `/help` | Mostra todos os comandos disponíveis |
| `/exit` | Encerra a sessão |
| `/clear` | Limpa a tela da conversa |
| `/compact` | Resume a conversa para economizar memória |
| `/cost` | Mostra quanto você gastou na sessão atual |
| `/status` | Mostra informações sobre a sessão |

**Experimente agora:**
```
/help
```

---

## Como o Claude pede sua aprovação

Antes de **modificar qualquer arquivo**, o Claude Code mostra o que vai fazer e pede confirmação:

```
Claude: Vou criar o arquivo relatorio.txt com o seguinte conteúdo:
        "Relatório de Vendas - Janeiro 2024..."
        
        Posso continuar? [Y/n]
```

- Digite `Y` (ou apenas Enter) para aprovar
- Digite `n` para cancelar
- O Claude **nunca age sem sua aprovação** em operações que modificam arquivos

---

## A arte de fazer boas perguntas

O Claude Code entende linguagem natural, mas pedidos mais específicos geram resultados melhores.

### Seja específico sobre o resultado que quer

❌ Vago:
```
> Organiza meus arquivos
```

✅ Específico:
```
> Tenho arquivos .jpg e .png misturados na pasta atual. 
  Crie duas subpastas: "fotos-jpg" e "fotos-png" e mova 
  cada arquivo para a pasta correspondente.
```

### Forneça contexto relevante

❌ Sem contexto:
```
> Esse código não funciona
```

✅ Com contexto:
```
> O arquivo app.py está dando erro quando eu rodo. 
  O erro diz "ModuleNotFoundError: No module named 'pandas'". 
  Pode me ajudar?
```

### Confirme antes de ações irreversíveis

Se você não tiver certeza, peça uma prévia:
```
> Antes de qualquer alteração, me mostre O QUE você faria, 
  sem executar ainda.
```

---

## Exercícios práticos desta sessão

Abra o terminal, crie uma pasta e entre nela:
```
mkdir exercicio-modulo3
cd exercicio-modulo3
claude
```

**Exercício 1 — Exploração:**
```
> Que arquivos existem nesta pasta?
```

**Exercício 2 — Criação de arquivo:**
```
> Crie um arquivo chamado notas.txt com 3 ideias de negócios fictícias
```

**Exercício 3 — Leitura:**
```
> Leia o arquivo notas.txt que você criou e me faça um resumo de cada ideia
```

**Exercício 4 — Edição:**
```
> Adicione ao final do arquivo notas.txt uma quarta ideia: "Serviço de entrega de livros usados"
```

**Exercício 5 — Reflexão:**
```
> Qual dessas 4 ideias você acha mais viável e por quê?
```

---

## Dica: o Claude tem memória durante a sessão

Dentro de uma mesma sessão (enquanto você não fechar com `/exit`), o Claude lembra de tudo que foi dito. Você pode referenciar coisas anteriores:

```
> Sobre aquele arquivo que você criou antes, pode renomeá-lo para ideias-negocio.txt?
```

Mas ao iniciar uma nova sessão (`claude` do zero), a memória é zerada — ele começa sem saber o que foi feito antes.

---

## Checklist

- [ ] Entendi os comandos especiais com `/`
- [ ] Sei como aprovar e rejeitar ações do Claude
- [ ] Fiz os 5 exercícios práticos
- [ ] Entendi que o Claude tem memória apenas dentro da sessão

**Próximo módulo →** [Módulo 4: Trabalhando com arquivos e pastas](modulo-04-arquivos-e-pastas.md)
