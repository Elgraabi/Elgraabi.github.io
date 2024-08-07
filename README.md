# Portfólio do Gabriel Oliveira

## Oi! 👋

Este é um site que mostra quem é o Gabriel Oliveira e as habilidades dele como desenvolvedor. Vamos aprender sobre o que cada parte do código faz!

### Estrutura do Site

Nosso site é feito de duas partes principais:
1. **Bio (Biografia)**: Onde a gente conhece o Gabriel.
2. **Sobre (About)**: Onde ele fala sobre o que sabe e o que gosta de fazer.

### Código HTML

O HTML é a "esqueletão" do nosso site. Ele organiza e dá estrutura. Vamos ver as partes importantes:

#### `<head>`: Cabeça do Site

Aqui, a gente coloca coisas que não aparecem na tela, mas ajudam nosso site a funcionar bem:
- **Título**: O nome que aparece na aba do navegador.
- **Fontes**: Letras bonitas do Google.
- **Ícones**: Pequenas imagens para redes sociais e tecnologias.
- **CSS**: O estilo do site, que está no arquivo `styles.css`.

#### `<body>`: Corpo do Site

Aqui é onde as coisas aparecem na tela. Vamos ver as partes:

1. **Bio Container**: Fica do lado esquerdo.
   - **Nome e Foto**: Mostra quem é o Gabriel.
   - **Apresentação**: Um pequeno texto sobre ele.
   - **Boas-vindas**: Diz "Seja bem-vindo!".
   - **Redes Sociais**: Links para Facebook, LinkedIn e Instagram.
   - **E-mail**: Um jeito de mandar mensagens para o Gabriel.

2. **About Container**: Fica do lado direito.
   - **Nome e Título**: Mostra o nome e a profissão do Gabriel.
   - **Descrição**: Fala sobre o que ele gosta de fazer e aprender.
   - **Botão de Projetos**: Um botão para ver os projetos do Gabriel no GitHub.
   - **Skills (Habilidades)**: Lista das tecnologias que o Gabriel sabe usar.

### Código CSS

O CSS é como a roupa do nosso site. Ele deixa tudo bonito e organizado. Vamos ver algumas partes importantes:

#### Reset
```css
* {
    padding: 0;
    margin: 0;
    font-family: 'Roboto', sans-serif;
    box-sizing: border-box;
}
```
- **Reset**: Isso tira todos os espaçamentos padrões e coloca a fonte 'Roboto'.

#### Variáveis
```css
:root {
    --main-color: #54B689;
    --main-text-color: #FFF;
    --border-color: #999;
    --bio-bg-color: #1E2A3A;
    --bio-border-color: #293544;
    --about-bg-color: #111821;
}
```
- **Variáveis**: Essas são como apelidos para cores. Assim fica fácil usar as mesmas cores em várias partes do site.

#### Geral
```css
.highlight {
    color: var(--main-color);
}
```
- **Destaque**: Deixa as palavras importantes em verde.

#### Containers
```css
#container {
    display: flex;
    flex-direction: row;
    color: var(--main-text-color);
}
#bio-container {
    flex: 1 1 20%;
    min-height: 100vh;
    background-color: var(--bio-bg-color);
    text-align: center;
    padding: 30px 12px;
    border-right: 5px solid var(--bio-border-color);
}
#about-container {
    flex: 1 1 80%;
    min-height: 100vh; 
    background-color: var(--about-bg-color);
    padding: 50px;
}
```
- **Containers**: Eles dividem o site em duas partes, a bio e o sobre.

#### Mobile
```css
@media(max-width: 450px) {
    #container {
        flex-direction: column;
    }
    #bio-container {
        min-height: auto;
        border-right: none;
        border-bottom: 5px solid var(--bio-border-color);
    }
    #bio-container h2 {
        display: none;
    }
    #bio-container p {
        max-width: 60%;
        margin: 10px auto;
    }
    #about-container {
        text-align: center;
        padding: 30px;
    }
    #about-container .description {
        margin: 10px auto;
        max-width: 100%;
        line-height: 26px;
    }
    #btn-projects {
        margin: 20px auto;
    }
    .skills-box{
        flex: 1 1 100%;
        max-width: 100%;
        margin-bottom: 40px;
        text-align: left;
    }
    .skills-box i {
        font-size: 60px;
    }
}
```
- **Mobile**: Deixa o site bonito em telas pequenas, como celulares.

### Conclusão

Este é o site do portfólio do Gabriel Oliveira! Ele mostra quem ele é, o que ele sabe fazer e como entrar em contato com ele. O HTML organiza tudo e o CSS deixa tudo bonito. Espero que você tenha gostado de aprender sobre isso!

Se tiver alguma dúvida, pode perguntar! 😊
```
