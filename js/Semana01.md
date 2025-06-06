# Referência JavaScript Básico e Estruturas

---

## 1.1 Variáveis e Tipos

### let, const vs var
- **var**: escopo de função, sofre hoisting (declarado no topo da função), pode causar bugs.
- **let**: escopo de bloco, não sofre hoisting da mesma forma, permite reatribuição.
- **const**: escopo de bloco, não pode ser reatribuído (imutável no que se refere ao identificador), mas objetos internos podem ser mutáveis.

**Quando usar:**
- Prefira `const` por padrão.
- Use `let` quando precisar reatribuir a variável.
- Evite `var` para evitar confusões com escopo.

---

### Hoisting e Temporal Dead Zone (TDZ)
- **Hoisting**: declarações `var`, funções são "movidas" para o topo do escopo durante a compilação.
- **TDZ**: `let` e `const` são "hoisted" mas não podem ser acessados antes da declaração (gera erro).

```js
console.log(x); // undefined (var)
var x = 10;

console.log(y); // ReferenceError (let)
let y = 20;
```

---

### Tipos Primitivos
- `string`: texto, ex: `'olá'`
- `number`: números, ex: `42`, `3.14`
- `boolean`: `true` ou `false`
- `null`: ausência intencional de valor
- `undefined`: valor padrão não definido
- `symbol`: identificadores únicos
- `bigint`: números inteiros grandes, ex: `123n`

---

### Type coercion e comparações

- `==` faz coerção de tipos antes da comparação.
- `===` compara valor e tipo (mais seguro).

```js
0 == false;  // true
0 === false; // false
null == undefined; // true
null === undefined; // false
```

---

### Template Literals (backticks)

```js
const nome = 'João';
const mensagem = `Olá, ${nome}!`;
console.log(mensagem); // Olá, João!
```

- Permite interpolação e strings multilinha.

---

## 1.2 Estruturas de Dados

### Arrays

**Métodos essenciais:**

- `push()`, `pop()`, `shift()`, `unshift()`
- `map()`, `filter()`, `reduce()`
- `forEach()`

**Spread Operator:**

```js
const arr1 = [1, 2];
const arr2 = [...arr1, 3, 4]; // [1, 2, 3, 4]
```

---

### Objects

- Sintaxe básica:

```js
const pessoa = {
  nome: 'Ana',
  idade: 25
};
```

- **Computed Properties:**

```js
const chave = 'nome';
const obj = {
  [chave]: 'João'
};
console.log(obj.nome); // João
```

- **Shorthand:**

```js
const nome = 'Maria';
const idade = 30;

const pessoa = { nome, idade }; // mesma coisa que { nome: nome, idade: idade }
```

---

### Maps e Sets

- **Map:** coleção de pares chave-valor, preserva a ordem de inserção, aceita qualquer tipo como chave.

```js
const mapa = new Map();
mapa.set('chave', 'valor');
console.log(mapa.get('chave')); // valor
```

- **Set:** coleção de valores únicos.

```js
const conjunto = new Set([1, 2, 2, 3]);
console.log(conjunto); // Set { 1, 2, 3 }
```

---

### Destructuring

**Arrays:**

```js
const arr = [10, 20, 30];
const [a, b, c] = arr;
console.log(a, b, c); // 10 20 30
```

**Objects:**

```js
const obj = { nome: 'Ana', idade: 25 };
const { nome, idade } = obj;
console.log(nome, idade); // Ana 25
```

---

### Rest/Spread operators (`...`)

**Spread (desempacota elementos):**

```js
const nums = [1, 2, 3];
const novoArr = [...nums, 4, 5]; // [1, 2, 3, 4, 5]

const pessoa = { nome: 'Ana', idade: 25 };
const pessoaAtualizada = { ...pessoa, cidade: 'SP' };
```

**Rest (agrupa elementos):**

```js
function soma(...numeros) {
  return numeros.reduce((total, num) => total + num, 0);
}
console.log(soma(1, 2, 3)); // 6

const [primeiro, ...resto] = [10, 20, 30];
console.log(resto); // [20, 30]

const { nome, ...outros } = { nome: 'Ana', idade: 25, cidade: 'SP' };
console.log(outros); // { idade: 25, cidade: 'SP' }
```

---

**Fim da referência.**
