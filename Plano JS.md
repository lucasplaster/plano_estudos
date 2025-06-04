# Plano de Estudos: JavaScript Moderno (ES6+)

## 🎯 Objetivo
Aprender JavaScript moderno focando apenas na sintaxe e características específicas da linguagem, aproveitando conhecimento prévio em lógica de programação.

---

## 📚 FASE 1: Fundamentos Sintáticos (Semana 1-2)

### 1.1 Variáveis e Tipos
- `let`, `const` vs `var` (diferenças e quando usar)
- Hoisting e Temporal Dead Zone
- Tipos primitivos: `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint`
- Type coercion e comparações (`==` vs `===`)
- Template literals (backticks)

### 1.2 Estruturas de Dados
- **Arrays**: métodos essenciais, spread operator
- **Objects**: sintaxe, computed properties, shorthand
- **Maps** e **Sets** (estruturas modernas)
- **Destructuring**: arrays e objects
- **Rest/Spread operators** (`...`)

### 1.3 Funções Modernas
- Function declarations vs expressions
- **Arrow functions**: sintaxe e diferenças
- Parâmetros padrão e rest parameters
- Closures (conceito fundamental)
- Higher-order functions

---

## 🔧 FASE 2: Características Avançadas (Semana 3-4)

### 2.1 Programação Funcional
- **Array methods**: `map()`, `filter()`, `reduce()`, `forEach()`
- `find()`, `some()`, `every()`, `includes()`
- Chaining de métodos
- Imutabilidade vs mutabilidade

### 2.2 Orientação a Objetos Moderna
- **Classes ES6+**: constructor, métodos, getters/setters
- Herança com `extends` e `super`
- Static methods e properties
- Private fields (`#`)
- **Prototypes** (entender o sistema por trás)

### 2.3 Módulos ES6
- `import` e `export` (named e default)
- Dynamic imports
- Diferenças entre CommonJS e ES Modules

---

## ⚡ FASE 3: Programação Assíncrona (Semana 5-6)

### 3.1 Promises
- Criação e consumo de Promises
- `.then()`, `.catch()`, `.finally()`
- `Promise.all()`, `Promise.race()`, `Promise.allSettled()`
- Error handling em promises

### 3.2 Async/Await
- Sintaxe `async`/`await`
- Error handling com `try`/`catch`
- Async functions e return values
- Parallel vs Sequential execution

### 3.3 Fetch API
- Requisições HTTP modernas
- Trabalhando com JSON
- Headers e configurações
- Error handling em requests

---

## 🌐 FASE 4: JavaScript no Browser (Semana 7-8)

### 4.1 DOM Manipulation
- `querySelector()`, `querySelectorAll()`
- Criação e modificação de elementos
- Event listeners modernos
- Event delegation
- Template elements

### 4.2 Eventos Modernos
- `addEventListener()` vs inline events
- Event object e métodos
- Custom events
- Keyboard, mouse, form events

### 4.3 Web APIs Essenciais
- Local Storage / Session Storage
- Fetch API (aprofundamento)
- Console API
- History API (básico)

---

## 🔥 FASE 5: Recursos Avançados (Semana 9-10)

### 5.1 Novidades Modernas
- **Optional Chaining** (`?.`)
- **Nullish Coalescing** (`??`)
- **Logical Assignment** (`??=`, `||=`, `&&=`)
- Array methods novos: `at()`, `findLast()`
- `Object.entries()`, `Object.keys()`, `Object.values()`

### 5.2 Padrões Modernos
- **Destructuring avançado**
- **Module patterns**
- **Factory functions** vs Classes
- **Composition over inheritance**

### 5.3 Ferramentas e Ecossistema
- NPM e package.json (conceitos básicos)
- Babel e transpilação (entender o conceito)
- ESLint e formatação de código
- Bundlers (conceito geral)

---

## 🚀 FASE 6: Prática e Consolidação (Semana 11-12)

### 6.1 Projetos Práticos
- **Todo List** (CRUD completo com localStorage)
- **Weather App** (APIs externas)
- **Calculator** (eventos e DOM)
- **Quiz App** (arrays, objects, timer)

### 6.2 Code Review e Boas Práticas
- Clean Code em JavaScript
- Naming conventions
- Code organization
- Performance considerations básicas

---

## 📋 Cronograma Sugerido

**Tempo total**: 12 semanas (3 meses)
**Dedicação**: 1-2 horas por dia, 5-6 dias por semana

### Distribuição Semanal:
- **40%** - Teoria e conceitos
- **40%** - Prática com exercícios
- **20%** - Projetos e aplicação

---

## 🧪 EXPERIMENTOS PRÁTICOS POR FASE

### 🔬 FASE 1: Conversor de Dados Pessoais
**Objetivo**: Praticar variáveis, tipos e estruturas básicas

**Experimento**: Crie um "Personal Data Converter" que:
- Recebe dados de uma pessoa em diferentes formatos
- Converte e formata usando template literals
- Pratica destructuring e spread operators
- Trabalha com diferentes tipos de dados

```javascript
// Exemplo do que você vai construir:
const userData = ["João", "Silva", 25, true, "Desenvolvedor"];
const userObject = { nome: "Maria", sobrenome: "Santos", idade: 30 };

// Converter, formatar e exibir de diferentes formas
// Usar template literals, destructuring, etc.
```

**Entregável**: Uma função que recebe dados em array/object e retorna uma bio formatada.

---

### 🔬 FASE 2: Sistema de Biblioteca Digital
**Objetivo**: Dominar programação funcional e POO

**Experimento**: Construa um gerenciador de livros que:
- Use classes para `Book`, `Author`, `Library`
- Implemente métodos funcionais para filtrar/buscar
- Pratique herança com diferentes tipos de livros
- Use módulos para organizar o código

```javascript
// Funcionalidades que você vai implementar:
library.addBook(book);
library.findBooks(criteria);
library.getBooksByAuthor(author);
library.getBooksByGenre(genre);
// Usar map, filter, reduce extensively
```

**Entregável**: Sistema completo com classes e métodos funcionais para gerenciar coleção de livros.

---

### 🔬 FASE 3: Monitor de Criptomoedas
**Objetivo**: Dominar programação assíncrona

**Experimento**: Crie um dashboard que:
- Busca preços de criptomoedas em APIs reais
- Atualiza dados a cada X segundos
- Gerencia múltiplas requisições simultâneas
- Trata erros de conexão graciosamente

```javascript
// APIs que você vai usar (gratuitas):
// CoinGecko API ou CryptoCompare API
// Implementar com async/await e Promise.all()
```

**Entregável**: Dashboard funcional que monitora pelo menos 5 criptomoedas em tempo real.

---

### 🔬 FASE 4: Quiz Interativo Dinâmico
**Objetivo**: Dominar manipulação de DOM e eventos

**Experimento**: Desenvolva um quiz que:
- Carrega perguntas dinamicamente
- Cria elementos DOM via JavaScript
- Gerencia eventos de mouse/teclado
- Implementa timer e animações simples
- Salva resultados no localStorage

```javascript
// Funcionalidades principais:
// - Navegação por teclado (setas, enter, escape)
// - Criação dinâmica de elementos
// - Feedback visual imediato
// - Sistema de pontuação
```

**Entregável**: Quiz completo com pelo menos 10 perguntas, navegação fluida e persistência de dados.

---

### 🔬 FASE 5: Calculadora Científica Avançada
**Objetivo**: Aplicar recursos modernos do JavaScript

**Experimento**: Construa uma calculadora que:
- Use optional chaining para operações complexas
- Implemente nullish coalescing para valores padrão
- Aplique novos métodos de array para histórico
- Organize código com módulos modernos

```javascript
// Recursos modernos que você vai usar:
const result = calculator.memory?.lastOperation?.result ?? 0;
const history = operations.findLast(op => op.type === 'scientific');
// Usar Object.entries(), logical assignment, etc.
```

**Entregável**: Calculadora com operações básicas, científicas, conversões de base e histórico completo.

---

### 🔬 FASE 6: Gerenciador de Tarefas Completo
**Objetivo**: Integrar todos os conhecimentos

**Experimento**: Desenvolva um TODO App avançado que:
- Combine todas as técnicas aprendidas
- Implemente drag & drop
- Use Web APIs (notifications, geolocation)
- Tenha sincronização com API externa
- Seja uma PWA básica

```javascript
// Funcionalidades avançadas:
// - Categorias dinâmicas
// - Filtros complexos
// - Backup/restore de dados
// - Modo offline
// - Notificações do sistema
```

**Entregável**: Aplicação completa e profissional que demonstre domínio total do JavaScript moderno.

---

## 📋 Como Executar os Experimentos

### Estrutura de Cada Experimento:
1. **Dia 1-2**: Planejamento e setup inicial
2. **Dia 3-5**: Implementação core features
3. **Dia 6-7**: Refinamento e extras
4. **Revisão**: Code review próprio e melhorias

### Critérios de Aprovação:
- ✅ Funcionalidade completa implementada
- ✅ Código usa conceitos da fase específica
- ✅ Sem erros no console
- ✅ Interface responsiva e funcional
- ✅ Código comentado e organizado

### Ferramentas por Experimento:
- **Fases 1-2**: Apenas JavaScript puro + HTML básico
- **Fase 3**: JavaScript + HTML + CSS + APIs externas
- **Fases 4-5**: JavaScript + DOM + CSS + Web APIs
- **Fase 6**: Stack completo + considerações PWA

---

## 🛠️ Recursos Recomendados

### Documentação
- MDN Web Docs (referência principal)
- JavaScript.info (tutorial completo)
- Can I Use (compatibilidade de browsers)

### Prática
- Codepen.io (experimentação rápida)
- VS Code com extensões JS
- Browser DevTools (debugging)

### Exercícios
- FreeCodeCamp (JavaScript section)
- Codewars (algoritmos)
- LeetCode (estruturas de dados)

---

## ✅ Marcos de Progresso

- **Semana 2**: Consegue escrever funções básicas e manipular arrays/objects
- **Semana 4**: Domina programação funcional e classes
- **Semana 6**: Trabalha confortavelmente com código assíncrono
- **Semana 8**: Manipula DOM e eventos sem dificuldade
- **Semana 10**: Usa recursos modernos do JavaScript fluentemente
- **Semana 12**: Desenvolve projetos completos independentemente

---

## 🎓 Objetivo Final

Ao final deste plano, você terá domínio completo da sintaxe moderna do JavaScript e estará preparado para:
- Desenvolver aplicações front-end
- Trabalhar com frameworks (React, Vue, etc.)
- Entender e contribuir em projetos JavaScript
- Continuar aprendizagem com Node.js ou frameworks específicos