
# 📘 Declaração de Variáveis em C
## Material preparado pelo Prof. Hudson Neves

---

## 🎯 Objetivo
Este material apresenta uma introdução clara e prática sobre **declaração de variáveis em C**, abordando:
- O que é uma variável
- Como declarar e inicializar variáveis
- Tipos mais comuns
- Regras de nomenclatura
- Uso com `scanf` e `printf`
- Exemplos práticos
- Exercícios

---

# 🧠 1. O que é uma variável?
Uma **variável** é um espaço reservado na memória do computador para armazenar um valor que pode mudar ao longo do programa.

Exemplo conceitual:
- Variável `idade` → armazena um número inteiro
- Variável `altura` → armazena um valor decimal

---

# 🧱 2. Como declarar variáveis em C
A declaração segue o padrão:
```
tipo nome;
```
Ou com inicialização:
```
tipo nome = valor;
```

### Exemplos:
```c
int idade;
float altura;
char letra;
double salario = 4500.75;
```

---

# 🧩 3. Regras de nomenclatura de variáveis
✔️ Deve começar com letra ou `_`  
✔️ Pode conter números, letras e `_`  
✔️ Diferencia maiúsculas e minúsculas (`idade` ≠ `Idade`)  
❌ Não pode começar com número  
❌ Não pode conter espaço  
❌ Não pode ser palavra reservada

### Exemplos válidos:
```c
int contador;
float media_final;
char _codigo;
```

### Exemplos inválidos:
```c
int 2valor;      // começa com número
float salário;   // acento
char nome completo; // espaço
```

---

# 🔄 4. Declaração, inicialização e atribuição
### Declaração:
```c
int idade;
```
### Inicialização:
```c
int idade = 20;
```
### Atribuição:
```c
idade = 30;
```

---

# 🧮 5. Principais tipos de variáveis
### Inteiros
```c
int ano = 2026;
short dia = 27;
unsigned int alunos = 40;
```

### Ponto flutuante
```c
float temperatura = 26.5;
double distancia = 98765.4321;
```

### Caractere
```c
char letra = 'A';
```

### Booleano
```c
#include <stdbool.h>
bool ativo = true;
```

---

# 📥 6. Entrada de dados (scanf)
```c
int idade;
printf("Digite sua idade: ");
scanf("%d", &idade);
```

Tabela de especificadores:
| Tipo | Código |
|------|--------|
| int | %d |
| float | %f |
| double | %lf |
| char | %c |
| bool | %d |

---

# 📤 7. Saída de dados (printf)
```c
printf("Idade: %d", idade);
printf("Altura: %.2f", altura);
```

---

# 🎬 8. Exemplo completo
```c
#include <stdio.h>
#include <stdbool.h>

int main() {
    int idade;
    float altura;
    char inicial;
    bool matriculado = true;

    printf("Digite sua idade: ");
    scanf("%d", &idade);

    printf("Digite sua altura: ");
    scanf("%f", &altura);

    printf("Digite sua inicial: ");
    scanf(" %c", &inicial);

    printf("
--- Dados Informados ---
");
    printf("Idade: %d
", idade);
    printf("Altura: %.2f
", altura);
    printf("Inicial: %c
", inicial);
    printf("Matriculado: %d
", matriculado);

    return 0;
}
```

---

# 🎓 9. Erros comuns
❌ Usar variável sem inicializar  
❌ Nome inválido  
❌ Confundir tipos (ex: usar `%d` com `float`)  
❌ Esquecer `&` no `scanf`  
❌ Esquecer `;`

---

# 📝 10. Exercícios
### **1. Declare variáveis para:**
- nome (char)
- idade (int)
- salário (float)
- aprovado (bool)

### **2. Leia valores do usuário e imprima formatado.**

### **3. Declare uma variável sem valor e atribua valores diferentes a ela.**

### **4. Corrija o código a seguir:**
```c
float numero;
scanf("%d", numero)
char letra = A;
int 3alunos;
```

---

# ✔️ Aula concluída!

Próximo conteúdo sugerido: operadores aritméticos e condicionais.

