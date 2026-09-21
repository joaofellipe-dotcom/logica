# Estruturas de Repetição e Páginas Estáticas no GitHub

Este documento apresenta conceitos essenciais para o desenvolvimento de software, divididos entre a lógica de programação estruturada e a publicação de projetos na Web.

---

## Parte 1: Estruturas de Repetição na Lógica de Programação

As **estruturas de repetição** (ou *loops*) permitem que um conjunto de instruções seja executado repetidamente enquanto uma determinada condição for verdadeira ou até que se atinja um número definido de iterações.

### 1. Por que usar Estruturas de Repetição?
* **Automação:** Executar a mesma tarefa milhares de vezes com poucas linhas de código.
* **Redução de Código:** Evita a repetição manual de instruções (princípio DRY - *Don't Repeat Yourself*).
* **Manipulação de Dados:** Essencial para percorrer listas, matrizes e arrays.

### 2. Tipos Principais de Estruturas

#### A. Repetição com Teste no Início (`Enquanto` / `While`)
Avalia uma condição lógica **antes** de executar o código. Se for falsa no início, o bloco não é executado nenhuma vez.
* **Pseudocódigo:**
  ```text
  Enquanto (condição for verdadeira) Faça
      // Instruções a serem repetidas
  FimEnquanto
  ```

#### B. Repetição com Teste no Fim (`Repita...Até` / `Do...While`)
Executa o bloco de código **pelo menos uma vez** antes de avaliar a condição no final.
* **Pseudocódigo:**
  ```text
  Repita
      // Instruções a serem repetidas
  Até que (condição seja verdadeira)
  ```

#### C. Repetição com Variável de Controlo (`Para` / `For`)
Possui um mecanismo integrado para inicializar um contador, testar uma condição e atualizar essa variável a cada iteração. Ideal quando o número de repetições é conhecido fixamente.
* **Pseudocódigo:**
  ```text
  Para contador De valor_inicial Até valor_final Passo incremento Faça
      // Instruções a serem repetidas
  FimPara
  ```

---

## Parte 2: Criação de Páginas Estáticas no GitHub

O **[GitHub Pages](https://docs.github.com/pt/pages/getting-started-with-github-pages/what-is-github-pages "O que é o GitHub Pages?")** é um serviço gratuito de alojamento oferecido pelo GitHub que permite transformar repositórios de código em sites acessíveis diretamente pelo navegador.

### 1. O que é uma Página Estática?
Uma **página estática** é um site composto por ficheiros que são entregues ao navegador do utilizador exatamente como estão armazenados no servidor (geralmente arquivos **HTML, CSS e JavaScript**). 
* Ao contrário dos sites dinâmicos (como WordPress ou sistemas em PHP/Python), as páginas estáticas **não processam dados num servidor** e não se ligam diretamente a uma base de dados no momento do acesso.
* São altamente seguras, rápidas e ideais para portfólios, documentações de projetos ou páginas institucionais.

### 2. Como Funciona a Publicação no GitHub Pages?
O processo de publicação baseia-se no conteúdo guardado num repositório público da sua conta. Existem duas abordagens principais para criar o endereço URL do site:

1. **Site de Utilizador:** O repositório deve ter obrigatoriamente o nome exato `<seu-utilizador>.github.io`. O site ficará disponível na raiz desse domínio.
2. **Site de Projeto:** Pode utilizar qualquer repositório. O endereço final seguirá o formato `<seu-utilizador>.github.io/<nome-do-repositorio>`.

### 3. Passo a Passo para Criar e Publicar a sua Página

Para colocar um site estático no ar através da interface Web do GitHub, siga estas etapas:

1. **Criar o Repositório:** Aceda ao [GitHub](https://github.com/ "GitHub Official Website"), crie um novo repositório e configure-o como **Público**.
2. **Enviar os Ficheiros:** Adicione os ficheiros do seu site (como o design em CSS e scripts JS). É obrigatório que o ficheiro principal da página inicial se chame exatamente **`index.html`** e esteja localizado na raiz do repositório.
3. **Ativar o Serviço:**
   * Entre nas **Settings** (Configurações) do seu repositório.
   * No menu lateral esquerdo, clique na secção **Pages**.
   * Na opção *Build and deployment*, defina a *Source* como **Deploy from a branch**.
   * Escolha a branch principal (geralmente `main` ou `master`), selecione a pasta `/root` e clique em **Save**.
4. **Aceder ao Site:** O GitHub Actions iniciará o processo de compilação. Em poucos minutos, uma barra verde surgirá no topo da mesma página de configurações exibindo o link público do seu site.
