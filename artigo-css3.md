###Unoesc Chapecó
###Pós-Graduação em Desenvolvimento Web, Cloud e Dispositivos Móveis - WebMob
###Disciplina: HTML5+CSS3
###Professor: Jean Carlo Nascimento
###Acadêmico(a): Eduardo Binda

###Artigo de Revisão de CSS3
</br></br>
##Introdução CSS3
</br>
  O CSS(Cascading Style Sheets) é um mecanismo pelo qual se pode aplicar estilos às páginas web. Como o ambiente de desenvolvimento web sofre diariamente constantes transformações em seu meio, as aplicações estão exigindo cada vez mais poder dos navegadores. Para isso surgiu o CSS3 a mais recente evolução do CSS onde com ele é possível construir animações, rotações, movimentos e transições tanto em 2D como em 3D deixando as páginas web mais interativas e intuitivas para o usuário. O CSS3 é totalmente compatível com as versões mais antigas do CSS. Para que o CSS3 possa funcionar corretamente é necessário que os browsers(navegadores) dêem suporte a tal funcionalidade. A maioria dos navegadores modernos como:Google Chrome, Mozzila Firefox, Opera, Safari e Internet Explorer já dispõem de suporte a esta nova tecnologia.  

####Referências:
http://www.w3schools.com/css/css3_intro.asp
http://www.w3.org/Style/CSS/
http://blog.caelum.com.br/css3-e-o-futuro-da-web/

###Funcionalidade: calc()
#####O que é?
A funcionalidade calc() permite que possam ser definidos valores CSS com uso de cálculos (expressões) matemáticas, ou seja, o valor definido para a propriedade CSS é o resultado de uma expressão matemática.Os operadores matemáticos permitidos são: + (soma), - (subtração), * (multiplicação) e / (divisão).  Na expressão matemática que define o valor CSS é permitido que se misture diferentes unidades de medida. Vale destacar que nas operações de adição(+) e subtração(-) é necessário inserir um espaço em branco antes e depois do operador.
#####Onde usar?
As unidades de medida CSS válidas podem ser usadas em componentes que possuem as seguintes propriedades: comprimento, ângulo, tempo, frequência e números inteiros e fracionários.
#####Como usar?
	seletor { propriedade: calc(expressão matemática); }
#####Exemplo de uso
	div {
	 width: 90%;                /* para navegadores que não suportam calc() */
	 width: calc(100% - 100px); /* para suporte nativo */
	 margin: 0 auto;
	 height: 200px;
	 border: 1px solid black ;
	 background: lime;
	}	
#####Referências:http://www.maujor.com/tutorial/css3-funcao-css-calc.php



###Funcionalidade: text-shadow
#####O que é?
 É uma funcionalidade na qual dispõe de um efeito de sombreamento em textos.
#####Onde usar?
 Pode ser utilizado em elementos de texto com h1,h2,h3, etc...
#####Como usar?
	seletor { 
	text-shadow: param-1 param-2 param-3 cor; 
	} 

Onde:
param-1: é o deslocamento da sombra para a direita (caso o valor seja positivo) ou para a esquerda (caso o valor seja negativo);
param-2: é o deslocamento da sombra para baixo (caso o valor seja positivo) ou para cima (caso o valor seja negativo);
param-3: é o raio para um efeito blur na sombra;
cor: é a corque será dada à sombra.
#####Exemplo de uso
	h1 {
	    font-size:30px; 
	    color:black; 
	    text-shadow: 2px -2px lime; 
	    }	
#####Referências:http://www.maujor.com/tutorial/css3-text-shadow.php, http://www.w3schools.com/cssref/css3_pr_text-shadow.asp

###Funcionalidade: box-shadow
#####O que é?
 É uma funcionalidade na qual permite fazer um efeito de sombra em boxes(caixas).
#####Onde usar?
 Pode ser utilizado em elementos como divs.
#####Como usar?
	seletor { box-shadow: inset offsetX offsetY raioBlur spread cor; }
#####Exemplo de uso
	div {
	    box-shadow: 10px 10px 5px #888888;
	}	
#####Referências:http://www.w3schools.com/cssref/css3_pr_box-shadow.asp, http://www.maujor.com/tutorial/interativo-css3/

###Funcionalidade: resize
#####O que é?
 É uma funcionalidade na qual permite com que determinado elemento possa ser redimencionado pelo usuário.
#####Onde usar?
 Pode ser utilizado em elementos como divs.
#####Como usar?
	seletor { resize: horizontal;
              overflow: auto; 
          	}
O usuário pode informar através dos parâmetro resize se o redimencionamento do elemento será feito de forma horizontal, vertical ou amabas.
#####Exemplo de uso
	div {
	    resize: horizontal;
	    overflow: auto;
	} 	
#####Referências:http://www.w3schools.com/css/css3_user_interface.asp

###Funcionalidade: RGBA
#####O que é?
 É uma nova funcionalidade do CSS3 que nos permite informarmos valores de cores RGB(Red, Green,Blue) e transparência(opacidade).
#####Onde usar?
 Pode ser utilizado em elementos que possuam propriedades que permitem que sejam informados valores para cores tais como: background, color, etc.
#####Como usar?
	seletor { background: rgba(92, 88, 89, 0.5); } 
Sabendo que os três parâmetros inciais(red,green,blue)são informados valores numéricos para as cores e no parâmetro alpha é informado um valor de 0 a 1 para definir a transparência(opacidade) ou também pode ser informado em (%).
#####Exemplo de uso
	div {
	     background-color: rgba(255,200,29,0.9);
	}	
#####Referências:http://www.maujor.com/tutorial/interativo-css3/inc/

###Funcionalidade: Transform 2D - skew
#####O que é?
 Essa funcionalidade dará um efeito de inclinação em um elemneto em relação aos seus eixos x e y. Podem ser informados valores tanto positivos quanto negativos para os ângulos(deg, grad, rad e turn) onde irá garantir a inclinação do elemento.
#####Onde usar?
 Pode ser aplicado em qualquer elemento html
#####Como usar?
	seletor { transform: skew(αdeg, βdeg); } 
#####Exemplo de uso
	div{
    width:100px;
    height:100px;
    background-color:green;
    transform: skew(30deg,30deg);
    -ms-transform: skew(30deg,30deg); /* IE 9 */
    -webkit-transform: skew(30deg,30deg); /* Safari e Chrome */
    -o-transform: skew(30deg,30deg); /* Opera */
    -moz-transform: skew(30deg,30deg); /* Firefox */
	}
#####Referências:http://www.maujor.com/tutorial/interativo-css3/, http://www.linhadecodigo.com.br/artigo/3487/transformacoes-2d-com-as-css3-propriedade-transform.aspx#ixzz3pCCsPHlk

###Funcionalidade: Transform 2D - rotate
#####O que é?
 Este método permite como o próprio nome diz rotacionar um determinado elemento com base em uma valor de ângulo passado por parâmetro.
#####Onde usar?
 Pode ser aplicado em elementos html do tipo div.
#####Como usar?
	seletor {transform: rotate(αdeg); }  
#####Exemplo de uso
	div{
	    width:100px;
	    height:100px;
	    background-color:green;
	transform: rotate(30deg);
	-ms-transform: rotate(30deg); /* IE 9 */
	-webkit-transform: rotate(30deg); /* Safari e Chrome */
	-o-transform: rotate(30deg); /* Opera */
	-moz-transform: rotate(30deg); /* Firefox */
	}
#####Referências:http://www.linhadecodigo.com.br/artigo/3487/transformacoes-2d-com-as-css3-propriedade-transform.aspx#ixzz3pFMb6OmB, http://www.maujor.com/tutorial/interativo-css3/

###Funcionalidade: Transform 2D - translate
#####O que é?
 Este nova funcionalidade do CSS3 permite com que se possa mover de lugar determinado elemento ao longo de seus eixos x e y.
#####Onde usar?
 Pode ser aplicado em elementos html do tipo div ou qualquer outro elemento que possa ser movimentado com base em seus eixos
#####Como usar?
	 seletor { transform: translate(x, y); } 
#####Exemplo de uso
	div{
	    width:100px;
	    height:100px;
	    background-color:green;
	    transform: translate(50px,100px);
	    -ms-transform: translate(50px,100px); /* IE 9 */
	    -webkit-transform: translate(50px,100px); /* Safari e Chrome */
	    -o-transform: translate(50px,100px); /* Opera */
	    -moz-transform: translate(50px,100px); /* Firefox */
	}
#####Referências: http://www.linhadecodigo.com.br/artigo/3487/transformacoes-2d-com-as-css3-propriedade-transform.aspx#ixzz3pFQOLA3Y, http://www.maujor.com/tutorial/interativo-css3/

###Funcionalidade: Web Fonts - @font-face
#####O que é?
 É uma funcionalidade nova do CSS3 onde pode-se especificar um tipo de fonte para ser utilizado em suas páginas web independente se esta fonte esteja ou não instalada localmente em seu computador.
#####Onde usar?
 Pode ser utilizado em qualquer elemento html que possa ser configurado a propriedade fonte.
#####Como usar?
	@font face {
	descritivo: valor;
	descritivo: valor;
	}   
#####Exemplo de uso
	@font-face {
		font-family: "RegencyScriptFLF Regular";
		src: url("http://site/fontes/RegencyScriptFLF-Regular.ttf");
		}

	p { font-family: "RegencyScriptFLF Regular", Cursive; }
#####Referências: http://www.maujor.com/tutorial/css3-@font-face.php, http://www.w3schools.com/css/css3_fonts.asp

###Funcionalidade: Linear Gradients
#####O que é?
  É uma funcionalidade que permite com se possa através de duas paradas de cores formar um tom de gradiente, dando um efeito suave entre as cores.
#####Onde usar?
 Pode ser utilizado em elementos que suportam propriedades  
#####Como usar?
	background: linear-gradient( direction , color-stop1 , color-stop2, ... );
#####Exemplo de uso
	#grad {
	  background: -webkit-linear-gradient(left top, red , blue); /* For Safari 5.1 to 6.0 */
	  background: -o-linear-gradient(bottom right, red, blue); /* For Opera 11.1 to 12.0 */
	  background: -moz-linear-gradient(bottom right, red, blue); /* For Firefox 3.6 to 15 */
	  background: linear-gradient(to bottom right, red , blue); /* Standard syntax */
	} 
#####Referências:http://www.w3schools.com/css/css3_gradients.asp, http://www.linhadecodigo.com.br/artigo/3603/css3-gradient-criando-planos-de-fundo-com-efeito-degrade.aspx


###Funcionalidade: Animations
#####O que é?
 Essa funcionalidade permite que determinado elemento mude seu estilo de forma gradual. As animaçõess são criadas apartir de keyframes que por sua vez descreve como será feita a animação do elemento.
#####Onde usar?
 Essa nova funcionalidade pode ser utilizada na maioria dos elementos HTML, sem qualquer utilização de animaçãoes feitas em Flash ou até mesmo em Javascript.
#####Como usar?
    @keyframes nomedaanimacao {
       seletores-keyframe { estilo css para esse determinado keyframe; }
    }
#####Exemplo de uso
	
	@keyframes example {
	    0%   {background-color: red;}
	    25%  {background-color: yellow;}
	    50%  {background-color: blue;}
	    100% {background-color: green;}
	}

	div {
	    width: 100px;
	    height: 100px;
	    background-color: red;
	    animation-name: example;
	    animation-duration: 4s;
	}
#####Referências: http://www.w3schools.com/css/css3_animations.asp, http://tableless.com.br/transition-e-animation/
