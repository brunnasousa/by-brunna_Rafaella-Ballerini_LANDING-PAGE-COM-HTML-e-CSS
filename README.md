# by-brunna_Rafaella-Ballerini_LANDING-PAGE-COM-HTML-e-CSS
estudando/treinando html e css com o video do youtube Rafaella-Ballerini_LANDING-PAGE-COM-HTML-e-CSS


HTML
<!DOCTYPE html>
<html lang="pt-BR">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Um bot que irá moderar e deixar a sua comunidade segura de um jeito fácil!">
  <title>Balle Bot - Modere a sua comunidade do Discord</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>
  <header class="cabecalho"> <!--cabeçalho-->
    <img class="cabecalho-imagem" src="logo.svg" alt="Logo da comunidade Ballerini">
    <nav class="cabecalho-menu"> <!--menu de navegação-->
      <a class="cabecalho-menu-item" href="https://discord.gg/wagxzStdcR">Comunidade Ballerini</a> <!--tag de ancora-->
      <a class="cabecalho-menu-item" href="https://www.youtube.com/watch?v=llF6vD-RljE&t=1435s&ab_channel=RafaellaBallerini">Tutorial</a>
      <a class="cabecalho-menu-item" href="https://github.com/rafaballerini/LandingPage">Open Source</a>
      <a class="cabecalho-menu-item" href="https://www.figma.com/file/myqP66iQwzjwjrIAJyyrip/BalleBot?node-id=2%3A2">Comandos</a>
    </nav>
  </header>

  <main class="conteudo">
    <section class="conteudo-principal">
      <div class="conteudo-principal-escrito">
        <h1 class="conteudo-principal-escrito-titulo">Balle Bot</h1>
        <h2 class="conteudo-principal-escrito-subtitulo">Deixe a sua comunidade segura de um jeito fácil</h2>
        <button class="conteudo-principal-escrito-botao">Me adicione!</button>
      </div>
      <img class="conteudo-principal-imagem"src="ballebot.svg" alt="Imagem da Balle Bot">
    </section>

    <section class="conteudo-secundario">
      <h3 class="conteudo-secundario-titulo">O que ela faz por você?</h3>
      <p class="conteudo-secundario-paragrafo">1. Cria um <strong>sistema de verificação capcha</strong> para novos membros garantirem que não são robôs</p>
      <p class="conteudo-secundario-paragrafo">2. Possui um <strong>sistema de banimento automático</strong> para links suspeitos que forem enviados na comunidade</p>
      <p class="conteudo-secundario-paragrafo">3. <strong>Sistema de avisos e banimento manual</strong>, para pessoas administradoras utilizarem</p>
    </section>
  </main>

  <footer class="rodape">  <!--rodapé-->
    <img class="rodape-imagem" src="ballerini.svg">
    <p>Treino - Brunna D. S. Sousa em 20/02/2022.</p>
  </footer>
</body>

</html>

<!--feito dia 20/02/2022 Brunna D. S. Sousa-->

CSS
@import url('https://fonts.googleapis.com/css2?family=Righteous&family=Sarala:wght@400;700&display=swap');

* { /*serve pra resetar o css*/
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
}

body{
    font-size: 100%;
    background: linear-gradient(68.15deg, #2F2325 16.62%, #8E5D52 85.61%);; /*fundo da pagina inteira*/
}

/*------------------------------------------------------*/

.cabecalho{
    display: flex; /*referencia ao flex box*/
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    padding: 24px;
}

.cabecalho-imagem{
    height: 72px;
}

.cabecalho-menu{
    display: flex;
    gap: 32px;
}

.cabecalho-menu-item{
    font-family: 'Sarala', sans-serif;
    color: #FFF2E7;
    font-weight: 400; /*o negrito - o quao forte*/
    font-size: 18px; /*tamanho da fonte*/

}

/*------------------------------------------------------------*/

.conteudo{
    margin-bottom: 48px; /*distancia entre o final do main pro começo do footer*/
    border-top: 0.4px solid #FFF2E7;
}

.conteudo-principal{
    display: flex;
    flex-direction: row;
    align-items: center; /*alinhando o texto com a imagem pra elas ficarem na mesma linha*/
    justify-content: space-around;
}

.conteudo-principal-escrito{
    display: flex;
    flex-direction: column; /*pra deixar ele em coluna ja que quando bota o display flex ele arruma automaticamente p linha*/
    gap: 32px;
}

.conteudo-principal-escrito-titulo{
    font-family: 'Righteous', cursive;
    font-weight: 400;
    font-size: 64px;
    color: #FFF2E7;
}

.conteudo-principal-escrito-subtitulo{
    font-family: 'Sarala', sans-serif;
    font-weight: 400;
    font-size: 24px;
    color:  #ECD6C4;
}

.conteudo-principal-escrito-botao{
    background-color: #ECD6C4;
    width: 180px;
    height: 60px;
    border: none;
    box-shadow: 4px 5px 4px rgba(0, 0, 0, 0.25); /*caixa de sombra*/   
    border-radius: 20px;

    font-family: 'Sarala', sans-serif;
    font-weight: 400;
    font-size: 24px;
    color: #2F2325;
}

.conteudo-principal-escrito-botao:hover{ /*botao quando passar o mouse*/
    background-color: rgba(236, 214, 196, 0.53);
}

.conteudo-principal-imagem{
    height: 430px;
}

/*-----*/

.conteudo-secundario{
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 24px;
    margin-top: 48px;
}

.conteudo-secundario-titulo{
    border-top: 0.4px solid #FFF2E7;    
    padding-top: 48px;

    font-family: 'Righteous', cursive;
    font-weight: 400;
    font-size: 24px;
    color: #FFF2E7;

    margin-bottom: 16px;;
}

.conteudo-secundario-paragrafo{
    font-family: 'Sarala', sans-serif;
    font-weight: 300;
    font-size: 18px;
    color: #ECD6C4;
}

/*--------------------------------------------------------------------------------*/

.rodape{
    padding: 32px;
    border-top: 0.4px solid #FFF2E7;
}

.rodape-imagem{
    height: 48px;
    display: block;
    margin: 0 auto;
}
