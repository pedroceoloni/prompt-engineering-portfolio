# Prompt: Refactor Code

## Objetivo
Refatorar um trecho de código para melhorar legibilidade, performance ou aderência a boas práticas — sem alterar o comportamento externo.

---

## Prompt completo

```
Você é um engenheiro de software sênior especializado em [LINGUAGEM].

Sua tarefa é REFATORAR o código abaixo seguindo estas diretrizes:
- Melhore a legibilidade e clareza
- Aplique boas práticas e padrões da linguagem [LINGUAGEM]
- Reduza duplicação de código (DRY)
- [DIRETRIZ ADICIONAL — ex: prefira funções puras, use nomes descritivos]

RESTRIÇÕES:
- NÃO altere a assinatura das funções públicas
- NÃO mude o comportamento observável
- NÃO adicione dependências externas

CÓDIGO ORIGINAL:
```[LINGUAGEM]
[COLE O CÓDIGO AQUI]
```

FORMATO DA RESPOSTA:
1. Liste brevemente os problemas encontrados (máximo 5 itens)
2. Apresente o código refatorado
3. Explique as mudanças mais importantes (máximo 3 parágrafos)
```

---

## Variáveis

| Variável | Descrição | Exemplo |
|----------|-----------|---------|
| `[LINGUAGEM]` | Linguagem de programação | `Python`, `TypeScript`, `Go` |
| `[DIRETRIZ ADICIONAL]` | Regra específica do projeto | `use async/await`, `sem classes` |
| `[COLE O CÓDIGO AQUI]` | Código a ser refatorado | seu código atual |

---

## Por que funciona

**Role prompting** (`engenheiro sênior`) calibra o nível de resposta — o modelo adota vocabulário técnico e opiniões mais assertivas.

**Constraints explícitas** (`NÃO altere...`) são críticas em refatoração: sem elas, o modelo pode "melhorar" a API pública e quebrar código que depende dela.

**Formato estruturado** (problemas → código → explicação) separa diagnóstico de solução, tornando o output fácil de revisar e aplicar.

---

## Variações

### Refatoração focada em performance
Substitua a linha de diretrizes por:
```
- Priorize performance: reduza complexidade de tempo e espaço
- Identifique e elimine operações desnecessárias em loops
- Prefira estruturas de dados mais eficientes quando aplicável
```

### Refatoração para um padrão específico
```
Refatore aplicando o padrão [PADRÃO — ex: Repository Pattern, Strategy Pattern].
Mostre como o código se encaixa no padrão escolhido.
```

---

## Exemplo de resultado esperado

**Input:** função Python com múltiplos ifs aninhados e variáveis com nomes `x`, `y`, `temp`

**Output esperado:**
1. Problemas: nomes não descritivos, lógica condicional complexa, sem early return
2. Código refatorado com nomes claros, guard clauses e dicionário de mapeamento
3. Explicação das 3 mudanças principais
