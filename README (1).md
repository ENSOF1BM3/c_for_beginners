
## Material preparado pelo Prof. Hudson Neves


# 📘 Tipos Primitivos, Tipos de Dados e Variáveis em C

## 🎯 Objetivo
Este documento apresenta os conceitos fundamentais para iniciantes em programação na linguagem C, abordando:

- O que são **tipos primitivos**
- Tipos de dados disponíveis na linguagem
- Declaração e uso de variáveis
- Exemplos práticos

---

# 🧱 1. O que são Tipos Primitivos?
Tipos primitivos são categorias básicas de dados que definem **o tipo de valor** que uma variável pode armazenar e **quanto espaço de memória** ela ocupará. Eles são a base da programação em C.

C possui quatro grupos principais:

1. **Inteiros (int)** – números sem parte decimal
2. **Ponto flutuante (float, double)** – números com casas decimais
3. **Caractere (char)** – um único símbolo
4. **Lógico (bool)** – verdadeiro ou falso

---

# 🗂️ 2. Tipos de Dados em C

## 🔢 2.1 Tipos Inteiros
Representam números inteiros:

```c
int idade = 20;
short ano = 2024;
long populacao = 7800000000;
unsigned int quantidade = 50;
```

Modificadores:
- `short`
- `long`
- `unsigned`

---

## 🔣 2.2 Tipos de Ponto Flutuante
Representam valores decimais:

```c
float preco = 10.99;
double distancia = 1234567.891011;
```

Diferença:
- `float` → menor precisão
- `double` → maior precisão

---

## 🔤 2.3 Tipo Caractere
Representa um único caractere:

```c
char letra = 'A';
char simbolo = '#';
```

---

## ✔️ 2.4 Tipo Lógico (bool)
Requer a biblioteca `stdbool.h`:

```c
#include <stdbool.h>
bool ativo = true;
bool finalizado = false;
```

---

# 📌 3. Variáveis

Variáveis são espaços na memória para armazenar valores.

## 3.1 Declaração de variáveis

```c
tipo nome = valor;
```

Exemplo:

```c
int numero = 10;
float altura = 1.75;
char inicial = 'H';
```

## 3.2 Regras para nomear variáveis
- Devem começar com letra ou `_`
- Não podem começar com número
- Sem espaços
- Sensíveis a maiúsculas/minúsculas

---

# 🖨️ 4. Entrada e saída de dados

```c
#include <stdio.h>

int main() {
    int idade;
    float salario;
    char inicial;

    printf("Digite sua idade: ");
    scanf("%d", &idade);

    printf("Digite seu salario: ");
    scanf("%f", &salario);

    printf("Digite sua inicial: ");
    scanf(" %c", &inicial);

    printf("
--- Dados Informados ---
");
    printf("Idade: %d
", idade);
    printf("Salario: %.2f
", salario);
    printf("Inicial: %c
", inicial);

    return 0;
}
```

---

# 🧪 5. Tamanho dos Tipos (sizeof)

```c
printf("int: %lu bytes
", sizeof(int));
printf("float: %lu bytes
", sizeof(float));
printf("char: %lu bytes
", sizeof(char));
printf("double: %lu bytes
", sizeof(double));
```

---

# 🏁 Conclusão
Compreender **tipos primitivos**, **tipos de dados** e **variáveis** é fundamental para dominar a linguagem C e avançar para estruturas, ponteiros, funções e muito mais.

---

# 📎 Próximos Passos
- Operadores aritméticos
- Condicionais (`if`, `switch`)
- Laços (`for`, `while`)
- Funções
- Arrays e strings

