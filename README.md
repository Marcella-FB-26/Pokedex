# POKEDEX

# INTRODUÇÂO

O projeto consiste em colocar números ou nomes dos pokemons na Pokedex e assim aparecer a imagem deles!

![hero-img](https://github.com/user-attachments/assets/4af14f04-26b1-492e-9d31-145680cc4c2e)

# TECNOLOGIAS UTILIZADAS
 
* HTML: linguagem de programação para contrução de pagina web.
* CSS: Linguagem de marcação que tem como função estilisar a pagina.
* JavaScript: Linguagem de programçao que "dá vida" ao site, dando ação a todas suas funções.

# REQUISITOS

Instalar o VScode para realizar o projeto

# ESTRUTURAÇÃO

O Head do site precisar estas tags, porque assim vai reconhecer nossa acentuação na palavras e conectar os arquivos CSS e JS basicamente.
``` py
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Links -->
  <link rel="shortcut icon" href="./images/favicon.png" type="image/x-icon">
  <link rel="stylesheet" href="./style/style.css">

  <!-- Main JS (defer para que o JS carregue somente depois do HTML) -->
  <script defer src="./js/script.js"></script>

  <title>Pokédex</title> 
</head>

```

# IMPORTAÇÕES 
Essa Const serve para chmara a API que iremos utilizar para mostrar as imagens e os nomes dos pokemons.
``` py
 // Faz uma requisição à API do Pokémon
  const APIResponse = await fetch(`https://pokeapi.co/api/v2/pokemon/${pokemon}`);
```
Essa utilizamos para importar uma fonte que combina mais com o projeto
``` py
* /* Importa a fonte 'Oxanium' do Google Fonts */
* @import url("https://fonts.googleapis.com/css?family=Oxanium:wgh@300;400;500;600;700;800&display=swap");
```

# ALGUMAS FUNCIONALIDADES
Essa tag serve para colocar a imagem da pokedex no site.
``` py
 <img src="./images/pokedex.png" alt="Pokédex" class="pokedex">
```
E aqui serve para darmos nomes nas tags, para arrumarmos dentro da imagem onde ficara o nome, peso, número e a imagem do pokemon.
``` py
    <img alt="Pokemón" class="pokemon__image">

    <h1 class="pokemon__data">
      <span class="pokemon__number"></span>
      <span class="pokemon__name"></span>
    </h1>

    <h1 class="pokemon__infos">
      <span class="pokemon__height"></span>
      <span class="pokemon__weight"></span>
    </h1>

    <form class="form">
      <input type="search" class="input__search" placeholder="Encontrar Pokémon" required>
      </label>
    </form>

```
