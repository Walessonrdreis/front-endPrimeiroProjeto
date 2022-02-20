# front-endPrimeiroProjeto
Usando classes para referenciar a tag, se essa possuir muitos componentes.

Para pegar a cor no PSD, basta pegar através do conta gota do photoshop.

o Primeiro passo no HTML é criar a tag header no body, que será o local onde ficará a logo, em fim o cabeçalho do projeto
O header irá segurar todo o conteúdo 

Logo após é necessário criar uma div que será responsável por receber as demais div do header.

No arquivo main css a primeira tag a ser estilizada foi a div principal header de class menu-principal, que recebeu a cor gerada do PSD, pega através do conta-gotas do PS, assim como a altura (height) que foi 60px. Seguindo o PSD é uma simulação de um trabalho onde o disign da empresa ja deu o tamanho e basta apenas codificar .

Ainda no css a tag body, o corpo da página recebe largura e altura( width e height )  100%, não é obrigatório, mas é sempre bom por

No HTML, foi adcionado a tag <main> que será a tag principal de todo conteúdo do header, e colocaremos a largura igual a do PSD,  que no nosso caso foi 980px.

Como a tag <main> não está no cento atribui um margin: 0 auto, pois se excecionarmos o elemento, mostra que tem margin de 8 px

O menu principal tem que sempre ocupar 100% da tela.

Segundo o PSD a logo deve ficar centralizada no cabeçalho do lado esquerdo, para isso usamos o padding para centralizar( para testar depois, da pra pegar altura da logo e altura do main e calcular o cento perfeitamente)

Próximo passo é pegar as imagens que representam as redes sociais
Elas serão colocadas em uma lista não ordenada <ul>, como são quatro imagens, usaremos quatro listas<li>, em cada lista teremos uma tag de link <a> para redirecionar a rede social

Ao realizarmos essa ação as imagens apareceram uma em  baixo da outra e como um ponto na frente.
No CSS iremos resolver esse problema, resentando os pontos que não precisamos usando display: inline-block; ou { list-style:none; }

um dos motivos para as imagens das redes socias não esta no rodapé superior é porque a logo está ocupando toda largura, diminuindo o valor de 100%  ele fica no lugar desejado.

Para adicionar espaço entre as imagens que estão presentes nas <li>  usaremos no css margin-left, onde em px é possível aumentar a distância entre elas

Uma coisa que é interessante ser feita é remover a barra horizontal que aparece na página que está sendo construida, basta remover a margin dada por padrão a tag <body> usando<margin: 0 auto;>
Edição do <header> a proxíma parte é a edição do menu do site.

adcionando mais uma tag <main> que recebe como class coL_100, a class tem o significado de coluna 100% para que o main ocupe todo espaço do site
Para remover o subrinhado da tag <a> retiramos o text decoration: <text-decoration: none;>
ALguns  navegadores possuem uma cong=figuração padrão, automaticamente adcionada, no caso do chrome por exemplio a tag<ul>, para isso utizaremos no css o <padding: 0px!important;> que vai sobrescrever a propriedade do navegador
com a propriedade <placeholder> a gente consegue atribuir um texto padão dentro do nosso input 

No PSD pode se observar que a cada palavra ao passar o mouse é receberar uma cor e parra isso precisamos encontrar o local e adcionarmos as css no nosso caso ficoi dessa forma: .<menu ul li a:hover {
  color: #00bac6;
}>

OBS: Um dos motivos de por as tags scripts no final do body é que alem de ser uma boa pratíca exixte uma lógica por traz, pois, se for colocado junto com o link do css, ele carregará primeiro que o css, pois o Css precisa ir tag por tag descrita para estilizar, por isso que as tag script deve ficar no final do body seguindo o padrão de carregamento, ele vai por cascata.

Na quarta aula começamos a usar JavaScript, para isso utilizamos um site http://kenwheeler.github.io/slick/
Nesse site possivel encontrar as animaçãoes prontas basta apenas, colocarmos as tags script encontrardas no proprio site com seus devidos caminhos no documento HTML para os scripts: <script type="text/javascript" src="https://code.jquery.com/jquery-1.11.0.min.js"></script>
  <script type="text/javascript" src="https://code.jquery.com/jquery-migrate-1.2.1.min.js"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/slick-carousel@1.8.1/slick/slick.min.js"></script>
  e     CSS:   <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/slick-carousel@1.8.1/slick/slick.css"/>  No arquivo js pegamos o código do modelo que queremos no noss caso foi : $('.slider-principal').slick();

  Colocando asimagens das cetas no banner: button.slick-prev {
    // Resetando a fonte
  font-size: 0px;
  removendo a borda
  border: none;
  //Adcionando o tamanho da largura da imagem, indo nas propriedades da propria imagem
  width: 25px;
  //Adicionando o tamanho da altura da imagem, indo nas propriedades da imagem
  height: 51px;
  // eixando a cou de fundo trsnsparente
  background-color: transparent;
  //Adicionado a imagem 
  background-image: url('../img/anterior.png');
}
Todo botão deve ter <position: absolute;>
Para o botão ser visivel em nosso site, logo, etc, é necessario usarmos <z-index> ele pernite que o elemento escolhido fique em cima de outros elementos. 
Com o position absolute ele vai ficar em um lugar que não vai depender de nada, uma div ou alguma tag que vá locomovelo, depois disso usados a tag <top>

para resovel o problema do scroll : .slick-list {
  width: 100%!important;
}
slick-initialized {
  overflow: hidden;
}







