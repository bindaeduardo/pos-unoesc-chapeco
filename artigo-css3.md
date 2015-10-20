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
