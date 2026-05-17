# Template de Prompt Genérico

Use este template como ponto de partida para qualquer novo prompt.

---

## Estrutura

```
## PAPEL (Role)
Você é [PAPEL ESPECÍFICO] com expertise em [DOMÍNIO].

## CONTEXTO
[Informações relevantes sobre a situação, usuário ou sistema]

## TAREFA
Sua tarefa é [VERBO DE AÇÃO + OBJETIVO CLARO].

## ENTRADA
[Como o usuário vai fornecer o input — texto, código, URL, etc.]

## RESTRIÇÕES
- [O que o modelo NÃO pode fazer]
- [Limites de escopo, tamanho, estilo]
- [Dependências ou compatibilidades]

## EXEMPLOS (opcional — few-shot)
Entrada: [exemplo de input]
Saída esperada: [exemplo de output]

---

Entrada: [segundo exemplo]
Saída esperada: [segundo output]

## FORMATO DE SAÍDA
Responda em [FORMATO — ex: JSON, Markdown, lista numerada, prosa].
Estrutura esperada:
[descreva ou mostre a estrutura do output]

## CRITÉRIOS DE QUALIDADE
Uma boa resposta deve:
- [critério 1]
- [critério 2]
- [critério 3]
```

---

## Checklist antes de usar o prompt

- [ ] O papel está específico o suficiente? (não apenas "assistente", mas "revisor de código Python sênior")
- [ ] As restrições negativas estão claras?
- [ ] O formato de saída está descrito?
- [ ] Há pelo menos 1 exemplo se o output for não-óbvio?
- [ ] O prompt é testável? (saberei quando a resposta é boa ou ruim?)

---

## Princípios de prompt engineering que sempre aplico

| Princípio | Por quê |
|-----------|---------|
| Seja específico no papel | Papéis genéricos geram respostas genéricas |
| Mostre exemplos (few-shot) | Exemplos calibram melhor que instruções longas |
| Diga o que NÃO fazer | Tão importante quanto dizer o que fazer |
| Defina o formato de saída | Facilita parsing e uso do output |
| Peça raciocínio explícito | "Pense passo a passo" melhora a qualidade em tarefas complexas |
| Itere com base em falhas | O melhor prompt é o resultado de múltiplos testes |
