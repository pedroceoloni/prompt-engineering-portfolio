# Prompt: Code Review

## Objetivo
Obter uma revisão técnica completa de um trecho de código, como se fosse um code review real em pull request — com foco em bugs, segurança, performance e manutenibilidade.

---

## Prompt completo

```
Você é um revisor de código experiente. Faça um code review detalhado do código abaixo.

CONTEXTO DO PROJETO:
- Linguagem: [LINGUAGEM]
- Tipo de aplicação: [TIPO — ex: API REST, script de automação, componente frontend]
- Nível de criticidade: [BAIXO | MÉDIO | ALTO — ex: ALTO para código em produção]

CÓDIGO PARA REVISAR:
```[LINGUAGEM]
[COLE O CÓDIGO AQUI]
```

Avalie nas seguintes dimensões e use o formato abaixo:

## 🐛 Bugs e erros potenciais
[liste problemas que podem causar comportamento incorreto]

## 🔒 Segurança
[vulnerabilidades, dados sensíveis expostos, validações faltando]

## ⚡ Performance
[operações custosas, queries N+1, alocações desnecessárias]

## 📖 Legibilidade e manutenção
[nomes ruins, funções longas, comentários faltando ou errados]

## ✅ Pontos positivos
[o que está bem feito — sempre inclua pelo menos 2 itens]

## 🎯 Prioridades
Ranqueie as 3 mudanças mais importantes a fazer primeiro.
```

---

## Variáveis

| Variável | Descrição | Exemplo |
|----------|-----------|---------|
| `[LINGUAGEM]` | Linguagem do código | `JavaScript`, `Python` |
| `[TIPO]` | Contexto da aplicação | `API REST com Express` |
| `[CRITICIDADE]` | Importância do rigor | `ALTO` para produção |

---

## Por que funciona

**Dimensões fixas** garantem que o modelo não pule áreas importantes. Sem essa estrutura, revisões tendem a focar só em estilo e ignorar segurança.

**Nível de criticidade** influencia o rigor: para código de produção, o modelo é mais conservador; para scripts internos, mais pragmático.

**Seção de pontos positivos** é intencional — evita que o output pareça um ataque e torna o feedback mais equilibrado e acionável.

---

## Variações

### Review focado em segurança (OWASP)
```
Foque exclusivamente nas 10 principais vulnerabilidades do OWASP.
Para cada risco encontrado, cite qual item do OWASP se aplica.
```

### Review com sugestões de código
```
Para cada problema encontrado, inclua um snippet de código mostrando
como corrigir. Use diff format: - linha atual, + linha sugerida.
```

### Review comparativo
```
Compare as duas implementações abaixo e recomende qual usar e por quê.
IMPLEMENTAÇÃO A: [código]
IMPLEMENTAÇÃO B: [código]
```
