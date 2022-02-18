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
