# 📓 Caderno Temático: JavaScript e TypeScript Básicos

> Projeto desenvolvido como parte do desafio de Inteligência Artificial da [DIO](https://www.dio.me/), utilizando o [NotebookLM](https://notebooklm.google.com/) como ferramenta de aprendizagem ativa.

---

## 1. Contexto e Objetivos

**Tema escolhido:** Fundamentos de JavaScript e TypeScript

**Por que este tema?**
JavaScript é a base de toda a stack web moderna. TypeScript, por sua vez, adiciona tipagem estática e torna o código mais seguro e previsível — habilidade essencial para quem trabalha com React, Node.js e NestJS.

**Objetivos de estudo:**
- Consolidar conceitos fundamentais de JavaScript (tipos, funções, escopo, closures)
- Entender como o TypeScript se relaciona com o JavaScript (transpilação, tipos, interfaces)
- Identificar os erros mais comuns de iniciantes e como evitá-los
- Criar um material de revisão reutilizável para consulta futura

---

## 2. Curadoria de Fontes

As fontes abaixo foram selecionadas por serem abertas, confiáveis e com cobertura complementar entre si. Todas foram enviadas como documentos no NotebookLM.

| # | Fonte | Tipo | Link |
|---|-------|------|------|
| 1 | MDN Web Docs — JavaScript Guide | Documentação oficial | [link](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide) |
| 2 | You Don't Know JS Yet — Scope & Closures (Capítulos 1-3) | Livro open-source | [link](https://github.com/getify/You-Dont-Know-JS/tree/2nd-ed/scope-closures) |
| 3 | TypeScript Handbook — The Basics | Documentação oficial | [link](https://www.typescriptlang.org/docs/handbook/2/basic-types.html) |
| 4 | JavaScript.info — JavaScript Fundamentals | Tutorial interativo | [link](https://javascript.info/first-steps) |
| 5 | TypeScript Deep Dive (Basarat) — Why TypeScript | Livro open-source | [link](https://basarat.gitbook.io/typescript/getting-started/why-typescript) |
| 6 | Mini curso Javascript | Curso do canal Dev Club | [link](https://www.youtube.com/playlist?list=PLsFVybaG4mODFwCuV06yLitVTikKF09syt) |

---

## 3. Engenharia de Prompts e Cicatrizes

### 3.1 Prompts utilizados e respostas obtidas

**Prompt 1 — Visão geral do tema**
> *"Com base nas fontes carregadas, quais são os 5 conceitos mais importantes de JavaScript que um iniciante precisa dominar antes de aprender TypeScript?"*

**Resposta obtida:** O NotebookLM listou: (1) Variáveis e Tipos de Dados, (2) Funções, (3) Trabalhando com Objetos, (4) Coleções e Métodos de Array, (5)Controle de Fluxo e Lógica. Cada ponto veio referenciado com trechos das fontes.

**Avaliação:** Boa resposta, bem fundamentada. As referências às fontes foram precisas.

---

**Prompt 2 — Aprofundamento em um conceito**
> *"Explique o conceito de closure em JavaScript como se eu fosse um iniciante. Use um exemplo de código simples."*

**Resposta obtida:** O modelo explicou corretamente e trouxe um exemplo baseado no javascript.info. O exemplo foi claro, e o código estava formatado (com bloco de código markdown).



---

**Prompt 3 — Variação de prompt para comparação**
> *Versão A:* `"Qual a diferença entre JavaScript e TypeScript?"`
>
> *Versão B:* `"Com base no TypeScript Handbook e no TypeScript Deep Dive, liste as 3 principais vantagens práticas do TypeScript sobre o JavaScript puro para um desenvolvedor iniciante."`

**Comparação:** A versão A gerou uma resposta precisa baseada no contexto do conteúdo anexo ao notebookLM. A versão B manteve o padrão, com referências diretas às fontes. **Lição aprendida:** ser específico sobre qual fonte consultar e qual perfil de pessoa está perguntando melhora muito a qualidade da resposta.

---

**Prompt 4 — Geração de glossário**
> *"Com base em todas as fontes, gere um glossário com os 10 principais termos técnicos de JavaScript e TypeScript, com definição curta de uma frase para cada."*

**Resposta obtida:** Boa qualidade. Todos os termos estavam escritos da forma correta.

---

## 4. Miniguia de Estudo (Entrega Final)

### 4.1 Resumos estruturados

#### JavaScript — Conceitos Fundamentais

**Tipos de dados**
JavaScript tem 7 tipos primitivos: `string`, `number`, `bigint`, `boolean`, `undefined`, `null` e `symbol`. Além deles, existe o tipo `object` (que inclui arrays e funções). A tipagem é dinâmica — uma variável pode mudar de tipo em tempo de execução.

**Escopo e Hoisting**
`var` tem escopo de função e sofre hoisting (é "elevada" ao topo do escopo). `let` e `const` têm escopo de bloco e não sofrem hoisting da mesma forma. Prefira sempre `const`; use `let` quando precisar reatribuir.

**Funções e Arrow Functions**
Arrow functions (`=>`) são funções anônimas com sintaxe mais curta e sem `this` próprio — herdam o `this` do contexto externo. Funções tradicionais têm seu próprio `this`.

**Closures**
Uma closure é quando uma função "lembra" do escopo onde foi criada, mesmo após esse escopo ter encerrado. É a base de padrões como módulos, memoização e callbacks.

---

#### TypeScript — O que muda

**TypeScript é um superset de JavaScript.** Todo código JS válido é TS válido. O TS adiciona anotações de tipo que são removidas na transpilação — o output final é JS puro.

**Vantagens práticas:**
- Erros de tipo detectados antes de executar o código
- Autocompletar mais preciso no editor (VS Code)
- Contratos claros entre funções via interfaces e tipos

---

### 4.2 Glossário

| Termo | Definição |
|-------|-----------|
| **Hoisting** | Comportamento do JS de mover declarações de variáveis/funções para o topo do escopo antes da execução |
| **Closure** | Função que mantém acesso ao escopo onde foi criada, mesmo após esse escopo encerrar |
| **Escopo** | Contexto que determina onde uma variável pode ser acessada no código |
| **Arrow function** | Sintaxe curta para funções anônimas que herda o `this` do escopo externo |
| **Tipagem dinâmica** | Característica do JS onde o tipo de uma variável é definido em tempo de execução |
| **Tipagem estática** | Característica do TS onde os tipos são definidos em tempo de escrita/compilação |
| **Interface** | Contrato TypeScript que define a forma esperada de um objeto |
| **Transpilação** | Processo de converter código TypeScript em JavaScript antes de executar |
| **Type inference** | Capacidade do TypeScript de deduzir o tipo de uma variável sem anotação explícita |
| **`any`** | Tipo TypeScript que desativa a verificação de tipos — deve ser evitado quando possível |

---

### 4.3 Prompts reutilizáveis para revisão futura

```
// Revisão de conceito
"Explique [CONCEITO] em JavaScript como se eu fosse um iniciante. 
Use um exemplo de código em bloco formatado e cite qual fonte você usou."

// Comparação entre conceitos
"Qual a diferença prática entre [CONCEITO A] e [CONCEITO B]? 
Dê um exemplo de quando usar cada um."

// Geração de exercícios
"Com base nas fontes carregadas, crie 3 perguntas de fixação sobre [TEMA] 
com as respostas logo abaixo de cada pergunta."

// Identificação de erros comuns
"Quais são os 3 erros mais comuns que iniciantes cometem ao trabalhar com 
[CONCEITO]? Para cada erro, mostre o código incorreto e a versão corrigida."

// Resumo rápido
"Resuma [TEMA/FONTE] em no máximo 5 tópicos curtos, focando no que é 
mais importante para um desenvolvedor iniciante."
```

---

## Observações Finais

Este caderno foi construído com foco em **revisão ativa**: ao invés de apenas ler as fontes, os prompts foram elaborados para extrair comparações, exemplos práticos e aplicações reais. O registro das dificuldades (seção 3.2) é parte intencional do processo — errar no prompt e ajustar faz parte do aprendizado com IA.

---

*Projeto desenvolvido para o desafio de IA da [DIO](https://www.dio.me/) — utilizando [NotebookLM](https://notebooklm.google.com/) como ferramenta principal.*


## Link do NotebookLM

[BasicJS/TS](https://notebooklm.google.com/notebook/c983430d-6511-45e5-9384-c630dbda7810)