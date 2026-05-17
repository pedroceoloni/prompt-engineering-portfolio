# Prompt: Debug Assistant

## Objetivo
Diagnosticar erros e bugs de forma sistemática, entendendo a causa raiz antes de propor soluções.

---

## Prompt completo

```
Você é um especialista em debugging de [LINGUAGEM/FRAMEWORK].

Vou te apresentar um bug. Quero que você:
1. Analise o problema sistematicamente ANTES de propor qualquer solução
2. Identifique a causa raiz, não apenas o sintoma
3. Proponha a correção mínima necessária
4. Explique como evitar esse tipo de bug no futuro

AMBIENTE:
- Linguagem/Framework: [LINGUAGEM/FRAMEWORK]
- Versão: [VERSÃO]
- Sistema operacional: [SO — se relevante]

CÓDIGO COM BUG:
```[LINGUAGEM]
[COLE O CÓDIGO AQUI]
```

COMPORTAMENTO ATUAL (o que está acontecendo):
[DESCREVA O COMPORTAMENTO ERRADO]

COMPORTAMENTO ESPERADO (o que deveria acontecer):
[DESCREVA O COMPORTAMENTO CORRETO]

MENSAGEM DE ERRO (se houver):
```
[COLE O ERRO COMPLETO AQUI, incluindo stack trace]
```

PASSOS PARA REPRODUZIR:
1. [passo 1]
2. [passo 2]
3. ...

Agora analise e resolva o problema seguindo esta estrutura:

## Diagnóstico
[análise da causa raiz — por que isso está acontecendo]

## Correção
[código corrigido com explicação das mudanças]

## Como evitar no futuro
[padrão, lint rule, teste ou prática que previne esse bug]
```

---

## Variáveis

| Variável | Descrição | Exemplo |
|----------|-----------|---------|
| `[LINGUAGEM/FRAMEWORK]` | Tech stack | `Node.js com Express`, `Python 3.11` |
| `[VERSÃO]` | Versão específica | `18.2.0`, `3.11.4` |
| `[SO]` | Sistema operacional | `Ubuntu 22.04`, `macOS Sonoma` |

---

## Por que funciona

**Diagnóstico antes de solução** — ao instruir o modelo a analisar *antes* de propor correções, evitamos respostas apressadas que resolvem o sintoma mas não a causa raiz.

**Contexto de ambiente** — versão e SO são cruciais para bugs específicos de plataforma. Sem essa info, o modelo assume defaults que podem não se aplicar.

**Estrutura de reprodução** — forçar os passos de reprodução ajuda o modelo (e você!) a pensar sistematicamente sobre o problema.

**"Correção mínima necessária"** — essa instrução evita que o modelo reescreva metade do arquivo quando apenas uma linha precisa mudar.

---

## Variações

### Debug de performance (sem erro explícito)
```
Não há erro, mas o código está lento. Analise onde está o gargalo.
Use Big O notation para descrever a complexidade atual e a após a otimização.
TEMPO ATUAL: [ex: ~3s para 10k registros]
TEMPO ESPERADO: [ex: <500ms]
```

### Debug com hipóteses
```
Tenho 3 hipóteses sobre a causa do bug:
1. [hipótese 1]
2. [hipótese 2]
3. [hipótese 3]

Analise cada uma, diga qual é mais provável e por quê.
```

### Debug de testes falhando
```
Os testes abaixo estão falhando. Analise se o problema está
no código de produção ou nos próprios testes.
CÓDIGO: [código]
TESTES: [testes]
OUTPUT DOS TESTES: [output]
```
