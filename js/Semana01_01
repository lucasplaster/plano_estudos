# Referência JavaScript Básico e Estruturas

---

## 1.1 Variáveis e Tipos

### let, const vs var

| Palavra-chave | Escopo       | Hoisting           | Reatribuível         | Uso recomendado         |
|---------------|--------------|--------------------|----------------------|------------------------|
| `var`         | Função       | Sim (undefined)    | Sim                  | ❌ Evitar              |
| `let`         | Bloco        | TDZ (não acessível antes) | Sim            | ✅ Usar quando precisar reatribuir |
| `const`       | Bloco        | TDZ (não acessível antes) | Não (imutável referência¹) | ✅ Usar por padrão       |

¹ Objetos e arrays atribuídos a `const` podem ter seus conteúdos alterados, mas o identificador não pode ser reatribuído.

---

### Hoisting e Temporal Dead Zone (TDZ)

```
console.log(a); // undefined (var sofre hoisting)
var a = 10;

console.log(b); // ReferenceError (let/const TDZ)
let b = 20;

function foo() {
  console.log(c); // undefined (hoisting var)
  var c = 5;
}
foo();
```

- Declarações de `var` e funções são elevadas (hoisting).
- `let` e `const` também são elevadas, mas não podem ser usadas antes da declaração (TDZ).
- Acessar `let` ou `const` antes da declaração gera erro `ReferenceError`.

---

### Tipos Primitivos

| Tipo        | Exemplo           | Descrição                                       |
|-------------|-------------------|------------------------------------------------|
| `string`    | `'texto'`         | Cadeia de caracteres                            |
| `number`    | `42`, `3.14`      | Números, incluindo inteiros e decimais         |
| `boolean`   | `true`, `false`   | Valores lógicos                                |
| `null`      | `null`            | Ausência intencional de valor                   |
| `undefined` | `undefined`       | Valor padrão de variável não inicializada       |
| `symbol`    | `Symbol('id')`    | Identificador único e imutável                  |
| `bigint`    | `1234567890123n`  | Inteiros muito grandes                           |

**Observação:**  
```
typeof null === 'object'; // peculiaridade histórica do JS
```

---

### Type Coercion e Comparações

- `==` compara valores com coerção de tipos (pode gerar surpresas).
- `===` compara valor e tipo (recomendado para evitar bugs).

```
0 == false;         // true
0 === false;        // false
'5' == 5;           // true
'5' === 5;          // false
null == undefined;  // true
null === undefined; // false
```

- Prefira sempre `===` para evitar resultados inesperados.

---

### Template Literals (backticks)

Permitem interpolação de variáveis e expressões, e strings multilinha.

```
const nome = 'João';
const mensagem = `Olá, ${nome}!`;
console.log(mensagem); // Olá, João!

const multiline = `Linha 1
Linha 2
Linha 3`;
console.log(multiline);
```

---

## 1.2 Estruturas de Dados

### Arrays

Manipulação básica:

```
const arr = [1, 2, 3];

arr.push(4);       // adiciona ao final: [1,2,3,4]
arr.pop();         // remove do final: [1,2,3]
arr.shift();       // remove do início: [2,3]
arr.unshift(0);    // adiciona ao início: [0,2,3]

const dobrados = arr.map(n => n * 2);      // [2,4,6]
const pares = arr.filter(n => n % 2 === 0); // [2]
const soma = arr.reduce((acc, n) => acc + n, 0); // soma elementos
arr.forEach(n => console.log(n));          // itera sem retorno
```

#### Spread Operator em Arrays

```
const arr1 = [1, 2];
const arr2 = [...arr1, 3, 4]; // [1, 2, 3, 4]
```

---

### Objects

Sintaxe básica:

```
const pessoa = {
  nome: 'Ana',
  idade: 25
};
```

#### Computed Properties

Permite usar expressões como nome de chave:

```
const chave = 'nome';
const obj = { [chave]: 'João' };
console.log(obj.nome); // João
```

#### Shorthand Properties

Quando a chave e variável têm mesmo nome:

```
const nome = 'Maria';
const idade = 30;
const pessoa = { nome, idade }; // igual a { nome: nome, idade: idade }
```

---

### Maps e Sets

#### Map

Coleção chave-valor, aceita qualquer tipo de chave, mantém ordem de inserção.

```
const mapa = new Map();
mapa.set('chave', 'valor');
mapa.set(123, 'número');
console.log(mapa.get('chave')); // valor
console.log(mapa.has(123));     // true
mapa.delete('chave');
```

#### Set

Coleção de valores únicos, útil para eliminar duplicatas.

```
const conjunto = new Set([1, 2, 2, 3]);
console.log(conjunto); // Set {1, 2, 3}
conjunto.add(4);
console.log(conjunto.has(2)); // true
conjunto.delete(3);
```

---

### Destructuring

#### Arrays

```
const arr = [10, 20, 30];
const [a, b, c] = arr;
console.log(a, b, c); // 10 20 30

const [x, , z] = arr; // pula o segundo elemento
```

#### Objetos

```
const obj = { nome: 'Ana', idade: 25 };
const { nome, idade } = obj;
console.log(nome, idade); // Ana 25
```

#### Valores padrão e alias

```
const { nome: n = 'Sem nome', cidade = 'SP' } = { nome: 'Lucas' };
console.log(n, cidade); // Lucas SP
```

#### Destructuring aninhado

```
const usuario = {
  nome: 'João',
  endereco: {
    rua: 'Rua A',
    numero: 123
  }
};

const { endereco: { rua, numero } } = usuario;
console.log(rua, numero); // Rua A 123
```

---

### Rest e Spread Operators (`...`)

#### Spread

Expande elementos de array ou propriedades de objeto.

```
const nums = [1, 2, 3];
const novoArr = [...nums, 4, 5]; // [1, 2, 3, 4, 5]

const pessoa = { nome: 'Ana', idade: 25 };
const pessoaAtualizada = { ...pessoa, cidade: 'SP' };
// { nome: 'Ana', idade: 25, cidade: 'SP' }
```

#### Rest

Agrupa múltiplos elementos ou propriedades restantes.

```
function soma(...numeros) {
  return numeros.reduce((acc, n) => acc + n, 0);
}
console.log(soma(1, 2, 3)); // 6

const [primeiro, ...resto] = [10, 20, 30];
console.log(resto); // [20, 30]

const { nome, ...outros } = { nome: 'Ana', idade: 25, cidade: 'SP' };
console.log(outros); // { idade: 25, cidade: 'SP' }
```

---

**Fim da referência.**
