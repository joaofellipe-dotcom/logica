

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
