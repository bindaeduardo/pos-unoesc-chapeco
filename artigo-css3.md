###Unoesc Chapecó
###Pós-Graduação em Desenvolvimento Web, Cloud e Dispositivos Móveis - WebMob
###Disciplina: HTML5+CSS3
###Professor: Jean Carlo Nascimento
###Acadêmico(a): Eduardo Binda

###Artigo de Revisão de CSS3
</br></br>
##Introdução CSS3
</br>
  O CSS(Cascading Style Sheets) é um mecanismo pelo qual se pode aplicar estilos às páginas web, fazendo com que as mesmas se tornem mais interativas e dêem melhor aspecto visual para o usuário. O CSS3 é a mais nova evolução do CSS onde com ele é possível construir animações, rotações, movimentos e transições tanto em 2D como em 3D. O CSS3 é totalmente compatível com as versões mais antigas do CSS. Para que o CSS3 possa funcionar corretamente é necessários que os browsers(navegadores) dêem suporte a esta tal funcionalidade. A maioria dos navegadores mais modernos (Google Chrome, Mozzila Firefox, Opera, Safari e Internet Explorer) já dispõem de suporte a esta nova tecnologia.  

Referencia:
http://www.w3schools.com/css/css3_intro.asp
http://www.w3.org/Style/CSS/

###Funcionalidade: border-radius
#####O que é?
A propriedade CSS3 border-radius destina-se a definir bordas arredondadas. O arredondamento das bordas é feito com declaração de dois valores CSS de medida; o primeiro define o eixo horizontal (rx) de 1/4 de uma elipse e o segundo o eixo vertical (ry). O quarto de elipse assim definida é convenientemente inserida no canto vivo do box arredondando-o. O diagrama a seguir esclarece o esquema de arredondamento.
#####Onde usar?
Em qualquer elemento que possui o atributo border.
####Como usar?
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
#####Referencia:
http://www.maujor.com/tutorial/interativo-css3/inc/borderradius.php
