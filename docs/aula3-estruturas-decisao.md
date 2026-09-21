# Estruturas de Decisão na Lógica de Programação

Na programação, o código raramente é executado em uma linha reta do início ao fim. Muitas vezes, o programa precisa tomar decisões com base em condições operacionais. As **estruturas de decisão** (ou condicionais) permitem que o software escolha caminhos diferentes dependendo dos dados que recebe.

---

## 1. O que é uma Estrutura de Decisão?

Uma estrutura de decisão avalia uma expressão lógica (uma pergunta que só pode resultar em **Verdadeiro** ou **Falso**) e direciona o fluxo de execução para o bloco de código correspondente.

Pense nelas como **bifurcações em uma estrada**:
* Se o semáforo estiver verde, o carro **avança**.
* Caso contrário (se estiver vermelho), o carro **para**.

---

## 2. Tipos de Estruturas de Decisão

As três formas mais comuns de implementar a lógica de desvio de fluxo são:

### ⚡ Estrutura Simples (Se / If)
Executa um bloco de código **apenas se** a condição for verdadeira. Se for falsa, o programa ignora o bloco e segue em frente.
```pseudocode
SE (usuario_conectado == verdadeiro) ENTÃO
    Exibir ("Bem-vindo de volta!")
FIM_SE
```

### ↔️ Estrutura Composta (Se... Senão / If... Else)
Define dois caminhos possíveis. Um bloco roda se a condição for verdadeira, e o outro bloco obrigatoriamente roda se ela for falsa.
```pseudocode
SE (idade >= 18) ENTÃO
    Exibir ("Acesso liberado.")
SENÃO
    Exibir ("Acesso negado: menor de idade.")
FIM_SE
```

### 🛣️ Estrutura Encadeada (Se... Senão Se... / If... Else If...)
Utilizada quando existem múltiplas condições que precisam ser testadas em sequência. O programa testa a primeira; se for falsa, testa a segunda, e assim por diante.
```pseudocode
SE (nota >= 7) ENTÃO
    Exibir ("Aprovado!")
SENÃO SE (nota >= 5) ENTÃO
    Exibir ("Recuperação.")
SENÃO
    Exibir ("Reprovado.")
FIM_SE
```

---

## 3. Escolha Caso (Switch / Case)

Quando você precisa testar uma única variável contra uma lista de valores fixos específicos, a estrutura encadeada de `If... Else` pode se tornar confusa. Para isso, usamos o **Escolha Caso**.

```pseudocode
ESCOLHA (opcao_menu)
    CASO 1:
        Exibir ("Abrindo configurações...")
    CASO 2:
        Exibir ("Iniciando jogo...")
    CASO PADRÃO:
        Exibir ("Opção inválida.")
FIM_ESCOLHA
```

---

## 4. O papel dos Operadores Relacionais e Lógicos

Para criar as condições de teste dentro das estruturas de decisão, utilizamos operadores:

* **Operadores Relacionais (Comparações):** `==` (igual a), `!=` (diferente de), `>` (maior que), `<` (menor que), `>=` (maior ou igual), `<=` (menor ou igual).
* **Operadores Lógicos (Combinações):** `E` (todas as condições devem ser verdadeiras), `OU` (pelo menos uma condição deve ser verdadeira), `NÃO` (inverte o valor lógico).
