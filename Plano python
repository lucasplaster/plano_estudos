# Plano de Estudos: Python para Iniciantes Completos

## 🎯 Sobre Este Plano
Este plano foi criado especialmente para quem **nunca programou antes** e quer aprender Python do zero. Python é uma das linguagens mais fáceis para começar, com sintaxe clara e muito próxima do inglês.

**Tempo estimado**: 8-12 semanas (2-3 meses)  
**Dedicação**: 1 hora por dia, 5 dias por semana  
**Pré-requisitos**: Nenhum! Só curiosidade e vontade de aprender

---

## 🏗️ FASE 1: Primeiros Passos (Semana 1-2)

### 1.1 Configuração do Ambiente
**Objetivo**: Ter Python funcionando no seu computador

**O que fazer:**
- Instalar Python (versão 3.11 ou superior)
- Conhecer o IDLE (editor que vem com Python)
- Alternatively: instalar VS Code + extensão Python
- Testar se está funcionando: `print("Olá, mundo!")`

**Conceitos básicos:**
- O que é programação?
- Por que Python?
- Como executar código Python

### 1.2 Primeiros Comandos
**Conceitos fundamentais:**
- `print()` - mostrar texto na tela
- Comentários com `#`
- Python como calculadora
- Conceito de "executar" um programa

**Experimento prático:**
```python
# Crie um programa que:
print("Meu nome é [SEU NOME]")
print("Tenho", 25, "anos")  # substitua pela sua idade
print("2 + 2 =", 2 + 2)
print("10 * 5 =", 10 * 5)
```

---

## 📦 FASE 2: Variáveis e Tipos (Semana 2-3)

### 2.1 Variáveis
**Conceitos:**
- O que são variáveis (como "caixas" que guardam valores)
- Como criar variáveis: `nome = "João"`
- Regras para nomes de variáveis
- Reutilizar variáveis

### 2.2 Tipos de Dados Básicos
**Os 4 tipos principais:**
- **Texto (str)**: `"Olá"`, `'Python'`
- **Números inteiros (int)**: `42`, `100`, `-5`
- **Números decimais (float)**: `3.14`, `2.5`
- **Verdadeiro/Falso (bool)**: `True`, `False`

**Experimento prático: Calculadora Pessoal**
```python
# Crie variáveis com seus dados pessoais
nome = "Seu Nome"
idade = 25
altura = 1.75
estudante = True

# Calcule sua idade em dias
dias_vividos = idade * 365
print(f"{nome} já viveu aproximadamente {dias_vividos} dias!")

# Calcule quando você fará 100 anos
anos_para_100 = 100 - idade
print(f"Você fará 100 anos em {anos_para_100} anos")
```

---

## 💬 FASE 3: Interação com Usuário (Semana 3-4)

### 3.1 Input do Usuário
**Conceitos:**
- Função `input()` para receber dados
- Converter texto para números: `int()`, `float()`
- f-strings para formatação: `f"Olá, {nome}!"`

### 3.2 Operações Básicas
**Operadores matemáticos:**
- `+` (soma), `-` (subtração), `*` (multiplicação), `/` (divisão)
- `**` (potência), `//` (divisão inteira), `%` (resto)

**Experimento prático: Calculadora Interativa**
```python
# Programa que pergunta nome e idade, e faz cálculos
nome = input("Qual seu nome? ")
idade = int(input("Qual sua idade? "))

print(f"Olá, {nome}!")
print(f"Você nasceu em aproximadamente {2024 - idade}")
print(f"No próximo ano você terá {idade + 1} anos")

# Adicione mais cálculos interessantes!
```

---

## 🔀 FASE 4: Tomando Decisões (Semana 4-5)

### 4.1 Condicionais
**Conceitos:**
- Estrutura `if`, `elif`, `else`
- Operadores de comparação: `==`, `!=`, `>`, `<`, `>=`, `<=`
- Operadores lógicos: `and`, `or`, `not`

### 4.2 Comparações e Lógica
**Entendendo:**
- Como o computador toma decisões
- Verdadeiro vs Falso em programação
- Combinando condições

**Experimento prático: Classificador de Idade**
```python
nome = input("Qual seu nome? ")
idade = int(input("Qual sua idade? "))

print(f"Olá, {nome}!")

if idade < 13:
    print("Você é uma criança!")
elif idade < 18:
    print("Você é um adolescente!")
elif idade < 60:
    print("Você é um adulto!")
else:
    print("Você é um idoso sábio!")

# Adicione mais classificações (pode dirigir, pode votar, etc.)
```

---

## 🔄 FASE 5: Repetições (Semana 5-6)

### 5.1 Loop While
**Conceitos:**
- Repetir código enquanto condição for verdadeira
- Cuidado com loops infinitos
- Como sair de um loop

### 5.2 Loop For
**Conceitos:**
- Repetir um número específico de vezes
- Função `range()`: `range(10)`, `range(1, 11)`, `range(0, 10, 2)`
- Diferenças entre `while` e `for`

**Experimento prático: Jogo de Adivinhação**
```python
import random

numero_secreto = random.randint(1, 100)
tentativas = 0

print("🎯 Jogo de Adivinhação!")
print("Pensei em um número entre 1 e 100")

while True:
    palpite = int(input("Qual seu palpite? "))
    tentativas += 1
    
    if palpite == numero_secreto:
        print(f"🎉 Parabéns! Você acertou em {tentativas} tentativas!")
        break
    elif palpite < numero_secreto:
        print("📈 Muito baixo! Tente um número maior")
    else:
        print("📉 Muito alto! Tente um número menor")
```

---

## 📝 FASE 6: Listas (Semana 6-7)

### 6.1 Conceito de Listas
**Entendendo:**
- Listas como "caixas com vários compartimentos"
- Criar listas: `frutas = ["maçã", "banana", "laranja"]`
- Acessar itens: `frutas[0]`, `frutas[1]`
- Python conta a partir do 0!

### 6.2 Manipulando Listas
**Operações básicas:**
- Adicionar: `lista.append(item)`
- Remover: `lista.remove(item)`
- Tamanho: `len(lista)`
- Verificar se existe: `item in lista`

**Experimento prático: Lista de Compras Inteligente**
```python
lista_compras = []

print("📝 Lista de Compras Inteligente")
print("Digite 'sair' para terminar")

while True:
    item = input("Que item deseja adicionar? ")
    
    if item.lower() == 'sair':
        break
    
    if item in lista_compras:
        print(f"'{item}' já está na lista!")
    else:
        lista_compras.append(item)
        print(f"'{item}' adicionado à lista!")
    
    print(f"Lista atual: {lista_compras}")

print(f"\n🛒 Lista final com {len(lista_compras)} itens:")
for i, item in enumerate(lista_compras, 1):
    print(f"{i}. {item}")
```

---

## 🔧 FASE 7: Funções (Semana 7-8)

### 7.1 Criando Funções
**Conceitos:**
- Funções como "mini-programas" reutilizáveis
- Definir função: `def nome_funcao():`
- Chamar função: `nome_funcao()`
- Parâmetros e argumentos

### 7.2 Funções com Retorno
**Conceitos:**
- Palavra-chave `return`
- Funções que calculam e devolvem valores
- Diferença entre `print()` e `return`

**Experimento prático: Calculadora com Funções**
```python
def somar(a, b):
    return a + b

def subtrair(a, b):
    return a - b

def multiplicar(a, b):
    return a * b

def dividir(a, b):
    if b != 0:
        return a / b
    else:
        return "Erro: Divisão por zero!"

def calculadora():
    print("🧮 Calculadora Python")
    
    while True:
        print("\nOperações:")
        print("1. Somar")
        print("2. Subtrair") 
        print("3. Multiplicar")
        print("4. Dividir")
        print("5. Sair")
        
        escolha = input("Escolha uma operação (1-5): ")
        
        if escolha == '5':
            print("Até logo!")
            break
        
        if escolha in ['1', '2', '3', '4']:
            num1 = float(input("Digite o primeiro número: "))
            num2 = float(input("Digite o segundo número: "))
            
            if escolha == '1':
                resultado = somar(num1, num2)
            elif escolha == '2':
                resultado = subtrair(num1, num2)
            elif escolha == '3':
                resultado = multiplicar(num1, num2)
            elif escolha == '4':
                resultado = dividir(num1, num2)
            
            print(f"Resultado: {resultado}")
        else:
            print("Opção inválida!")

# Chamar a calculadora
calculadora()
```

---

## 📚 FASE 8: Trabalhando com Arquivos (Semana 8-9)

### 8.1 Lendo Arquivos
**Conceitos:**
- Abrir arquivo: `open("arquivo.txt", "r")`
- Ler conteúdo: `.read()`, `.readlines()`
- Sempre fechar arquivo ou usar `with`

### 8.2 Escrevendo Arquivos
**Conceitos:**
- Criar/escrever: `open("arquivo.txt", "w")`
- Adicionar: `open("arquivo.txt", "a")`
- Escrever texto: `.write()`

**Experimento prático: Diário Digital**
```python
import datetime

def adicionar_entrada():
    data_hoje = datetime.date.today()
    entrada = input("O que aconteceu hoje? ")
    
    with open("diario.txt", "a", encoding="utf-8") as arquivo:
        arquivo.write(f"{data_hoje}: {entrada}\n")
    
    print("✅ Entrada adicionada ao diário!")

def ler_diario():
    try:
        with open("diario.txt", "r", encoding="utf-8") as arquivo:
            conteudo = arquivo.read()
            if conteudo:
                print("📖 Seu diário:")
                print(conteudo)
            else:
                print("Diário vazio. Que tal escrever algo?")
    except FileNotFoundError:
        print("Ainda não há um diário. Crie uma entrada primeiro!")

def menu_diario():
    while True:
        print("\n📔 Diário Digital")
        print("1. Adicionar entrada")
        print("2. Ler diário")
        print("3. Sair")
        
        escolha = input("Escolha uma opção: ")
        
        if escolha == '1':
            adicionar_entrada()
        elif escolha == '2':
            ler_diario()
        elif escolha == '3':
            print("Até logo!")
            break
        else:
            print("Opção inválida!")

menu_diario()
```

---

## 🏆 PROJETO FINAL: Sistema de Cadastro Simples (Semana 9-10)

### Objetivo
Criar um programa que junte todos os conceitos aprendidos:

**Funcionalidades:**
- Cadastrar pessoas (nome, idade, cidade)
- Listar todas as pessoas
- Buscar pessoa por nome
- Salvar dados em arquivo
- Carregar dados do arquivo
- Menu interativo

**Este projeto deve usar:**
- ✅ Variáveis e tipos
- ✅ Input do usuário
- ✅ Condicionais (if/elif/else)
- ✅ Loops (while/for)
- ✅ Listas
- ✅ Funções
- ✅ Arquivos

---

## 📋 Cronograma de Estudos

### Rotina Diária Recomendada (1 hora):
- **15 min**: Revisar conceitos do dia anterior
- **30 min**: Aprender conceitos novos
- **15 min**: Praticar com exercícios

### Estrutura Semanal:
- **Segunda a Quinta**: Aprender conceitos novos
- **Sexta**: Praticar e fazer exercícios
- **Final de semana**: Experimento prático da fase

### Marcos de Progresso:
- **Semana 2**: Consegue criar variáveis e fazer cálculos
- **Semana 4**: Consegue criar programas que tomam decisões
- **Semana 6**: Consegue criar programas com repetições
- **Semana 8**: Consegue organizar código com funções
- **Semana 10**: Consegue criar um programa completo

---

## 🛠️ Ferramentas Necessárias

### Para Começar:
1. **Python 3.11+** (python.org)
2. **IDLE** (vem com Python)
3. **Bloco de notas** (para arquivos .py)

### Para Evoluir:
1. **VS Code** + extensão Python
2. **Git** (para versionar projetos)
3. **Terminal/Prompt** (para executar programas)

---

## 📚 Recursos de Apoio

### Documentação:
- Python.org - Tutorial oficial
- W3Schools Python - Exemplos práticos
- Real Python - Artigos detalhados

### Exercícios:
- HackerRank - Desafios básicos
- Codewars - Problemas graduais
- URI Online Judge - Exercícios brasileiros

### Comunidade:
- Stack Overflow - Dúvidas técnicas
- Reddit r/learnpython - Comunidade iniciante
- Discord Python Brasil - Chat em português

---

## 🎯 Dicas para o Sucesso

### ✅ Faça:
- **Pratique diariamente** (mesmo que 15 minutos)
- **Digite o código** (não apenas leia)
- **Experimente modificar** os exemplos
- **Comete erros** (faz parte do aprendizado!)
- **Peça ajuda** quando emperrar

### ❌ Evite:
- **Pular etapas** (cada conceito é importante)
- **Apenas copiar código** (tente entender)
- **Desistir no primeiro erro** (debugging é normal)
- **Comparar seu progresso** com outros
- **Estudar por horas seguidas** (melhor pouco e frequente)

---

## 🚀 Próximos Passos (Após completar este plano)

### Caminhos possíveis:
1. **Web Development**: Django, Flask
2. **Data Science**: Pandas, NumPy, Matplotlib
3. **Automação**: Selenium, scripts de sistema
4. **Jogos**: Pygame
5. **Mobile**: Kivy, BeeWare
6. **Desktop**: Tkinter, PyQt

### Conceitos avançados:
- Programação orientada a objetos
- Manipulação de APIs
- Bancos de dados
- Testes automatizados
- Deploy de aplicações

---

## 🎓 Certificado de Conclusão

Quando terminar este plano, você terá aprendido:
- ✅ Fundamentos da programação
- ✅ Sintaxe Python completa
- ✅ Resolução de problemas
- ✅ Boas práticas de código
- ✅ Criação de projetos completos

**Parabéns! Você agora é um programador Python!** 🐍✨

---

*"A jornada de mil milhas começa com um único passo. No caso da programação, começa com um simples `print('Hello, World!')`"* 

Boa sorte e bons estudos! 🚀
