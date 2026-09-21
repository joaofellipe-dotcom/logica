markdown# Variáveis e Tipos de Dados na Lógica de Programação

Na lógica de programação, entender como armazenar e manipular informações é o primeiro passo para criar qualquer software. Este guia explica os dois conceitos mais fundamentais: **variáveis** e **tipos de dados**.

---

## 1. O que é uma Variável?

Uma **variável** é um espaço na memória do computador reservado para armazenar um dado que pode ser modificado durante a execução do programa. 

Pense nela como uma **caixa etiquetada**:
* **O Nome (Identificador):** É a etiqueta da caixa (ex: `idade`). Serve para você encontrar o dado depois.
* **O Conteúdo (Valor):** É o que está dentro da caixa (ex: `25`).
* **A Atribuição:** É o ato de colocar algo na caixa. Na maioria das linguagens, usa-se o sinal de igual (`=`).

```pseudocode
idade = 25
```

---

## 2. Tipos de Dados Primitivos

Os dados que colocamos dentro das variáveis possuem naturezas diferentes. Os quatro tipos primitivos mais comuns são:

### 🔢 Inteiro (Integer)
Numeração sem casas decimais. Utilizado para contagens e quantidades exatas.
* **Exemplos:** `10`, `-5`, `1000`, `0`
* **Uso comum:** `total_itens = 5`

### 📐 Real / Ponto Flutuante (Float/Double)
Números com frações ou casas decimais.
* **Exemplos:** `3.14`, `19.99`, `-0.5`
* **Uso comum:** `preco_produto = 29.90`

### 🔤 Texto / Cadeia de Caracteres (String)
Qualquer conjunto de caracteres (letras, números, símbolos) delimitado por aspas.
* **Exemplos:** `"Olá, Mundo!"`, `"User123"`, `"5"` (aqui o 5 é texto, não número)
* **Uso comum:** `nome_usuario = "Ana"`

### ⚖️ Booleano / Lógico (Boolean)
Representa apenas dois estados possíveis: verdadeiro ou falso. Fundamental para tomadas de decisão.
* **Exemplos:** `true` (Verdadeiro), `false` (Falso)
* **Uso comum:** `usuario_logado = true`

---

## 3. Tipagem Estática vs. Tipagem Dinâmica

As linguagens de programação lidam com os tipos de duas formas principais:

* **Tipagem Estática:** Você deve declarar obrigatoriamente o tipo da variável antes de usá-la, e ela não pode mudar de tipo depois. (Ex: Java, C#, C++).
  ```c
  int idade = 30; // Sempre será um inteiro
  ```
* **Tipagem Dinâmica:** O tipo é inferido automaticamente pelo valor que você atribui. A mesma variável pode mudar de tipo ao longo do código. (Ex: Python, JavaScript).
  ```python
  idade = 30 # Aqui é um inteiro
  idade = "Trinta" # Agora virou um texto (String)
  ```

---

## 4. Boas Práticas para Criar Variáveis

Para que seu código seja legível e profissional, siga estas regras de ouro:

1. **Nomes semânticos:** Escolha nomes que expliquem o que a variável guarda. Use `preco_final` em vez de `p` ou `x`.
2. **Evite caracteres especiais:** Não use espaços, acentos ou cecidilha (`ç`) em nomes de variáveis.
3. **Padrões de escrita:** Escolha um padrão e siga-o:
   * `camelCase`: `dataNascimento`
   * `snake_case`: `data_nascimento`
4. **Sensibilidade a maiúsculas (Case Sensitive):** Lembre-se que `idade` e `Idade` são tratadas como duas variáveis totalmente diferentes na maioria das linguagens.
