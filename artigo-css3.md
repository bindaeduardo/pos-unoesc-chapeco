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

####Referencia:
http://www.w3schools.com/css/css3_intro.asp
http://www.w3.org/Style/CSS/
http://blog.caelum.com.br/css3-e-o-futuro-da-web/

###Funcionalidade: border-radius
#####O que é?
A propriedade CSS3 border-radius destina-se a definir bordas arredondadas. O arredondamento das bordas é feito com declaração de dois valores CSS de medida; o primeiro define o eixo horizontal (rx) de 1/4 de uma elipse e o segundo o eixo vertical (ry). O quarto de elipse assim definida é convenientemente inserida no canto vivo do box arredondando-o. O diagrama a seguir esclarece o esquema de arredondamento.
#####Onde usar?
Em qualquer elemento que possui o atributo border.
#####Como usar?
	seletor {border-radius:
	  [ <length> | <percentage> ]{1,4} [ / [ <length> | <percentage> ]{1,4} ]?);
	}	
#####Exemplo de uso
A sintaxe geral para aplicar borda arredondada é mostrada a seguir.
	seletor {
	  border-top-left-radius: rx ry;
	  border-top-right-radius: rx ry;
	  border-bottom-right-radius: rx ry;
	  border-bottom-left-radius: rx ry;
	}
#####Referencia: http://www.maujor.com/tutorial/interativo-css3/inc/borderradius.php


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
#####Referencia:http://www.maujor.com/tutorial/css3-funcao-css-calc.php

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
#####Referencia:http://www.maujor.com/tutorial/css3-text-shadow.php, http://www.w3schools.com/cssref/css3_pr_text-shadow.asp

###Funcionalidade: box-shadow
#####O que é?
 É uma funcionalidade na qual permite fazer um efeito de sombra em boxes(caixas).
#####Onde usar?
 Pode ser utilizado em elementos como divs.
#####Como usar?
	seletor { box-shadow: inset offsetX offsetY raioBlur spread cor; }
Com relação aos parâmetros segue a mesma linha de raciocínio da funcionalidade text-shadow, onde o primeiro parâmetro define o deslocamento horizontal da sombra, o segundo parametro o deslocamento vertical da sombra, o terceiro o efeito da sombra e o quarto a cor que será dada à sombra do elemento.
#####Exemplo de uso
	div {
	    box-shadow: 10px 10px 5px #888888;
	}	
#####Referencia:http://www.w3schools.com/cssref/css3_pr_box-shadow.asp, http://www.maujor.com/tutorial/interativo-css3/

