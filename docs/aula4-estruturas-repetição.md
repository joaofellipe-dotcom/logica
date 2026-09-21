# Estruturas de Repetição na Lógica de Programação

As **estruturas de repetição** (ou *loops*) são blocos fundamentais na lógica de programação. Elas permitem que um conjunto de instruções seja executado repetidamente enquanto uma determinada condição for verdadeira ou até que se atinja um número definido de iterações.

---

## 1. Por que usar Estruturas de Repetição?

* **Automação:** Executar a mesma tarefa milhares de vezes com poucas linhas de código.
* **Redução de Código:** Evita a repetição manual de instruções (princípio DRY - *Don't Repeat Yourself*).
* **Manipulação de Dados:** Essencial para percorrer listas, matrizes, arrays e bases de dados.

---

## 2. Tipos Principais de Estruturas

Existem três estruturas principais utilizadas na maioria das linguagens de programação.

### A. Repetição com Teste no Início (`Enquanto` / `While`)
Esta estrutura avalia uma condição lógica **antes** de executar o bloco de código. Se a condição for falsa logo no início, o código dentro do laço não é executado nenhuma vez.

* **Ideal para:** Quando não se sabe o número exato de vezes que a repetição deve ocorrer.
* **Pseudocódigo:**
  ```text
  Enquanto (condição for verdadeira) Faça
      // Instruções a serem repetidas
  FimEnquanto
  ```

### B. Repetição com Teste no Fim (`Repita...Até` / `Do...While`)
Esta estrutura executa o bloco de código **pelo menos uma vez** antes de avaliar a condição. A validação é feita no final do bloco.

* **Ideal para:** Situações onde a primeira execução é obrigatória (ex: menus de opções ou validação de entrada de dados).
* **Pseudocódigo:**
  ```text
  Repita
      // Instruções a serem repetidas
  Até que (condição seja verdadeira/falsa)
  ```

### C. Repetição com Variável de Controlo (`Para` / `For`)
Esta estrutura possui um mecanismo integrado para inicializar uma variável (contador), testar uma condição e atualizar essa variável (incremento ou decremento) a cada iteração.

* **Ideal para:** Quando se sabe exatamente o número de vezes que o bloco deve ser executado.
* **Pseudocódigo:**
  ```text
  Para contador De valor_inicial Até valor_final Passo incremento Faça
      // Instruções a serem repetidas
  FimPara
  ```

---

## 3. Conceitos Cruciais

### O Contador e o Acumulador
* **Contador:** Variável que incrementa ou decrementa um valor fixo (geralmente `+1`) a cada volta do laço para controlar o número de repetições.
* **Acumulador:** Variável que soma valores variáveis a cada iteração (ex: calcular o total de uma lista de compras).

### O Perigo do Loop Infinito
Um **loop infinito** ocorre quando a condição de paragem de um laço `While` ou `Do...While` nunca se torna falsa. Isto consome todos os recursos do sistema e faz com que o programa bloqueie.

* **Exemplo de erro clássico:** Esquecer de incrementar a variável de controlo dentro de um laço `While`.

---

## 4. Exemplo Prático (Comparativo)

Objetivo: Exibir os números de 1 a 3 no ecrã.

| Estrutura | Exemplo em Pseudocódigo |
| :--- | :--- |
| **While** | `i = 1`<br>`Enquanto (i <= 3) Faça`<br>&nbsp;&nbsp;&nbsp;&nbsp;`Escrever(i)`<br>&nbsp;&nbsp;&nbsp;&nbsp;`i = i + 1`<br>`FimEnquanto` |
| **For** | `Para i De 1 Até 3 Passo 1 Faça`<br>&nbsp;&nbsp;&nbsp;&nbsp;`Escrever(i)`<br>`FimPara` |
