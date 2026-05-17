<div align="center">

# 🤖 Prompt Engineering Portfolio
### @pedroceoloni

[![GitHub](https://img.shields.io/badge/GitHub-@pedroceoloni-181717?style=flat-square&logo=github)](https://github.com/pedroceoloni)
[![Focus](https://img.shields.io/badge/Focus-Prompt%20Engineering-6366f1?style=flat-square)]()
[![Status](https://img.shields.io/badge/Status-Active-22c55e?style=flat-square)]()

> Coleção de prompts, templates e estudos de caso focados em **geração de código** e **chatbots/agentes com IA**.

</div>

---

## 👋 Sobre este repositório

Este portfólio documenta minha jornada em Prompt Engineering — a arte de comunicar-se com modelos de linguagem de forma eficaz e estruturada. Aqui você encontra prompts reais, com explicações de por que funcionam e como adaptá-los.

**Áreas de foco:**
- 🖥️ Geração e revisão de código com IA
- 🤖 Design de chatbots e agentes conversacionais

---

## 📁 Estrutura do repositório

```
prompt-engineering-portfolio/
│
├── 📂 prompts/
│   ├── 📂 code-generation/       # Prompts para geração de código
│   │   ├── README.md
│   │   ├── refactor-code.md
│   │   ├── code-review.md
│   │   └── debug-assistant.md
│   │
│   └── 📂 chatbots/              # Prompts para chatbots e agentes
│       ├── README.md
│       ├── customer-support-bot.md
│       ├── onboarding-agent.md
│       └── persona-definition.md
│
├── 📂 templates/                  # Templates reutilizáveis
│   ├── prompt-template.md
│   └── system-prompt-template.md
│
└── 📂 assets/                     # Imagens e recursos visuais
```

---

## 🚀 Destaques

### 🖥️ Code Generation
| Prompt | Descrição | Técnicas usadas |
|--------|-----------|-----------------|
| [Refactor Code](./prompts/code-generation/refactor-code.md) | Refatora código mantendo comportamento | Chain-of-thought, constraints |
| [Code Review](./prompts/code-generation/code-review.md) | Revisão detalhada com sugestões | Few-shot, role prompting |
| [Debug Assistant](./prompts/code-generation/debug-assistant.md) | Diagnóstico e correção de bugs | Step-by-step reasoning |

### 🤖 Chatbots & Agentes
| Prompt | Descrição | Técnicas usadas |
|--------|-----------|-----------------|
| [Customer Support Bot](./prompts/chatbots/customer-support-bot.md) | Agente de suporte ao cliente | System prompt, persona |
| [Onboarding Agent](./prompts/chatbots/onboarding-agent.md) | Guia de integração de novos usuários | Few-shot, memory simulation |
| [Persona Definition](./prompts/chatbots/persona-definition.md) | Template de definição de persona | Role, tone, constraints |

---

## 🧠 Técnicas aplicadas

```
✅ Chain-of-Thought (CoT)     — instruo o modelo a pensar passo a passo
✅ Few-Shot Prompting          — forneço exemplos para calibrar o output
✅ Role Prompting              — defino papéis específicos ao modelo
✅ System Prompts              — configuração de contexto e persona
✅ Output Constraints          — controle preciso do formato de resposta
✅ Negative Prompting          — instruo o que o modelo NÃO deve fazer
```

---

## 📖 Como usar este repositório

Cada arquivo de prompt segue a estrutura:

1. **Objetivo** — o que o prompt resolve
2. **Prompt completo** — pronto para copiar e usar
3. **Variáveis** — campos para personalizar (`[VARIÁVEL]`)
4. **Por que funciona** — análise das técnicas aplicadas
5. **Variações** — adaptações para casos diferentes

---

## 🛠️ Modelos testados

| Modelo | Status |
|--------|--------|
| Claude 3.5 / 4 Sonnet | ✅ Testado |
| GPT-4o | ✅ Testado |
| Gemini 1.5 Pro | ✅ Testado |
| Llama 3 (local) | 🔄 Em progresso |

---

## 📫 Contato

Se quiser trocar ideias sobre Prompt Engineering, me encontra no GitHub: [@pedroceoloni](https://github.com/pedroceoloni)

---

<div align="center">

*Feito com curiosidade e muitas iterações* 🔁

</div>
