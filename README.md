# 📝 Convenção de Nomeações

## 💡 Sobre este Repositório
Este repositório foi criado para compartilhar boas práticas sobre como dar nomes às "coisas" na programação, especialmente no universo do **Front-End**. Aqui você vai encontrar dicas e exemplos sobre como nomear **commits**, **branches**, **classes HTML/CSS**, **variáveis** e **funções** em JavaScript ou TypeScript. **Tudo de maneira simples e prática**.

---

## 🚀 GitHub

### Commits
Quando você for escrever uma mensagem de commit, é importante ser **claro e objetivo**. Use verbos no **imperativo**, ou seja, descreva ações diretas.</br>
- Existem alguns **prefixos** que ajudam a identificar o tipo de mudança no código. Aqui estão os mais usados:
  ```bash
  feat: para novas funcionalidades.
  fix: para correções de bugs.
  chore: mudanças que não afetam diretamente o código (ex.: configurações).
  refactor: melhorias no código sem alterar o comportamento.
  test: adição ou modificação de testes.
  docs: mudanças na documentação.
  style: ajustes de estilo (espaços, indentação, etc.).

- Um exemplo seria algo como:
  ```bash
  feat: add login feature
  fix: correct header alignment
  refactor: optimize user authentication logic

### Branches
Para nomear branches, é legal ter um padrão que facilite identificar o objetivo daquela branch. Aqui vão alguns exemplos:
- Novas funcionalidades:
  ```bash
  feature/<descriptive-name> (exemplo: feature/user-authentication).
- Correções:
  ```bash
  fix/<descriptive-name> (exemplo: feature/user-authentication).
- Melhorias:
  ```bash
  enhancement/<descriptive-name> (exemplo: feature/user-authentication).
- Experimentos:
  ```bash
  experiment/<descriptive-name> (exemplo: feature/user-authentication).

### ChangeLog para Pull Requests
Para descrever as mudanças feitas em um pull request, um bom modelo é usar categorias. Um formato interessante é o **Keep a Changelog**, onde você separa o que foi adicionado, alterado, corrigido ou removido.
- Por exemplo:
  ```bash
  Added: Novas funcionalidades.
  Changed: Alterações significativas.
  Fixed: Correções de bugs.
  Removed: Funcionalidades removidas.
Não necessariamente você deve preencher todos os campos, o ideal é sempre documentar as atividades que você realizou, se você não removeu nenhuma funcionalidade, não precisa adicionar o campo "**Removed**" por exemplo!
- Exemplo de utilização:
  ```bash
  **Added**:
    Authentication.
    LoginPage.
    SignupPage.
  
  **Changed**:
    HomePage wiht new dashboards.
  
  **Fixed**:
    Button without ":hover" css.

---

## 🌐 HTML/CSS

### Nomeação de Classes
Quando você for criar classes no HTML, uma boa prática é usar o formato kebab-case. Nesse padrão, você usa **letras minúsculas e separa as palavras com hífens**.
- Exemplo de utilização no HTML:
  ```bash
  <body>
    <header class="header">
      <h1 class="title">Kebab Case</h1>
      <nav class="menu">
        <a href="#" class="menu-item">Home</a>
        <a href="#" class="menu-item">About</a>
        <a href="#" class="menu-item">Contact</a>
      </nav>
    </header>
  </body>
- Utilizando no CSS:
  ```bash
  .header {
    background-color: #333;
    color: #fff;
    padding: 1rem;
    text-align: center;
  
    .title {
      font-size: 1.5rem;
      margin: 0;
    }
  
    .menu {
      margin-top: 0.5rem;
  
      .menu-item {
        color: #fff;
        margin: 0 0.5rem;
        text-decoration: none;
      }
    }
  }

### Nomeação de IDs
Os IDs podem ser nomeados de **várias maneiras**, e você pode escolher a que achar melhor para o **seu projeto**.
- Exemplos dos modelos mais **utilziados** para nomeação de identificadores HTML:
  ```bash
  UpperCamelCase => IdHeaderLogin
  lowerCamelCase => idHeaderLogin
  kebab-case => id-header-login
  snake_case => id_header_login

- Caso seu projeto seja bem documento e a padronização seja bem aplicada, você ainda pode usar algumas variações mais **ousadas**, por exemplo:
  ```bash
  Id_HeaderLogin
  id_HeaderLogin

Mas lembre-se, a partir do momento em que você decidiu qual será o padrão de nomeação dos identificadores, **fique atento e sempre mantenha a padronização no projeto**!
   
---

## 💻 Programação (JavaScript/TypeScript)

### Variáveis
Para nomear variáveis, o padrão mais comum é o **camelCase**. Isso significa começar com letra minúscula e usar maiúsculas para separar palavras.
- Exemplo:
  ```bash
  var nomeUsuario: string;
  let contador: int;
  const isUserConnected: boolean;
  
Agora, uma dica muito importante: escolha nomes que façam sentido. Não use abreviações confusas ou difíceis de entender. Imagine que outra pessoa vai trabalhar no seu código. Você quer que ela entenda facilmente o que cada variável faz, certo?</br></br>

**Eduardo, como assim? Não entendi direito.**</br></br>

Imagine que você está desenvolvendo um software que provavelmente será atualizado ou reutilizado futuramente, provavelmente por outro programador (é complicado, eu sei). Portanto, você deve evitar ao máximo abreviar tudo que ver pela frente, deixe o código legível para seu futuro colega de profissão.
- Por exemplo:
  ```bash
  // Imagine que você está declarando uma variável que vai armazenar o número de maçãs douradas de uma cesta de supermercado

  // Opção 1
  let cdMaDr: int;

  // Opção 2
  let contadorMacaDourada: int;
No exemplo acima podemos ver a diferença entre nomeação sem e com abreviação extrema das variáveis.</br>

Claro que é totalmente viável abreviar as variáveis que são extremamente grandes, mas deixe tudo bem **documentado** com comentários no código!

### Funções
Para as funções, o padrão também costuma ser **camelCase**, mas algumas pessoas usam **UpperCamelCase**, começando com letra maiúscula.

Outro ponto importante é que o nome da função deve deixar claro o **que ela faz**. Funções que começam com "**get**" geralmente pegam informações. Já funções que começam com "**send**" costumam enviar algo.
- Exemplos
  ````bash
  function GetUserId(){}
  async function UpdateUserName(){}
  sendMessage();
  DeleteMacaDourada();
Se você seguir essas práticas, seu código vai ficar muito mais fácil de entender e manter!

---

Com essas dicas, espero que você consiga melhorar a organização e a legibilidade dos seus projetos. Bora codar! 🚀









  

  
