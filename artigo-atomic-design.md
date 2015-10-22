###Unoesc Chapecó
###Pós-Graduação em Desenvolvimento Web, Cloud e Dispositivos Móveis - WebMob
###Disciplina: HTML5+CSS3
###Professor: Jean Carlo Nascimento
###Acadêmico(a): Eduardo Binda
###E-mail:eduardobinda7@gmail.com

##Artigo Atomic Design
</br>
####Resumo
 Diariamente o universo de desenvolvimento web se depara com situações onde o seu público (os usuários) estão cada vez mais exigentes tratando-se de layout e design de suas páginas e/ou aplicações web. Essa preocupação com o design web fez com que fossem criadas novas metodologias e alterantivas que viessem suprir essa necessidade dos desenvolvedores. Com o surgimento do design responsivo a partir de 2010 surgiu uma nova perspectiva no âmbito de projetos de design e interfaces web. Novas técnicas, ferramentas, procedimentos foram idealizadas e criadas para facilitar e otimizar a vida do desenvolvedor front-end. Porém neste contexto, sabe-se ainda que por mais visível que seja a evolução e tenha facilitado muito a vida dos programadores, ainda falta um algo a mais que possa vir complementar e a agregar a forma com que se projete e crie designers e interfaces de forma mais produtiva, eficiente e interativa com o usuário.
 Mediante ao contexto informado, uma nova metodologia foi proposta chamada de Atomic Design ou em português "Design Atômico". Veja a seguir:
</br>
####O que é ?
 O Atomic Design é uma metodologia idealizada e criada pelo webdesigner Brad Frost que visa explicar como os diversos e diferentes componentes de uma página web podem interagir entre si e também a como criar sistemas de design. Segundo o mesmo, as páginas web nada mais são do que um conjunto de elementos que estão conectados entre si formando um sistema web. O nome desta metodologia surgiu de sua inspiração nas aulas de química onde analisou que os componentes das páginas tinham o comportamento semelhante à componentes de química como: átomos, moléculas e organismos. 
 Josh Duck exemplifica atrvés da imagem abaixo como pode ser representada a "Tabela Periódica dos elementos HTML" na metodologia do Atomic Design.
<img src="http://bradfrost.com/wp-content/uploads/2012/11/Screen-Shot-2012-11-13-at-5.15.05-PM.png">  
</br>
####Como funciona 
 Basicamente o Atomic Design funciona baseado em cinco níveis como mostra na imagem abaixo e que será explicada em seguida:
<img src="http://bradfrost.com/wp-content/uploads/2013/06/atomic-design.png">
Para exemplificar melhor a imagem acima na qual demostra o conceito de Atomic Design, podemos comparar a primeira etapa os "Átomos" como sendo as TAGs HTML ex:(inputs, buttons, labels, etc...). O passo seguinte é chamado de "Moléculas" que se trata da combinação dos átomos(tags), os "forms" HTML são um exemplo disso e de certa forma são a base de sustentação do sistema web. Seguindo o raciocínio, o passo subsequente é denominado "Organismos" que por sua vez são aglomerados de moléculas que juntas formam um conjunto ou seção mais complexa, como por exemplo o cabeçalho de uma página web. O próximo passo desta metodologia consiste nos "Modelos" que por sua vez são um conjunto de organismos que juntamente formarão uma página web. São através da etapa de modelos que os clientes começam a ter uma noção de como irá ficar o design de sua página web. Por fim mas não menor importante a última etapa desta metodologia se chama "Páginas" que são as reais instâncias dos modelos efetuados na etapa anterior. Neste momeneto é que o usuário vê de forma real/tangível o resultado de sua página web.
</br>
####Por que usar, quais seus benefícios
 O uso do Atomic Design é recomendado para ser usado mais em sistemas web do que em sites devido a não ser tão necessário reutilizar os códigos dos componentes. 
 Uma das vantagens de se utilizar o Atomic Design é que o mesmo possui uma metodologia clara e objetiva de como construir sistemas de design e também de como conseguir visualizar e apreciar o resultado partindo do abstrato(o que se está projetando) para o concreto(aquilo que foi feito). Outra vantagem que pode ser destacada é a capacidade de escalabilidade do sistema onde você pode criar elementos que se comportam adequadamente a sua própria necessidade. Pensando na equipe de design de um sistema, pode-se apontar mais uma vantagem do uso do Atomic Design sendo que ele permite que se possa vizualizar o sistema como um todo sem a necessidade de ficar verificando e analisando os layouts salvos ou feitos em outra ferramenta. 
</br>
####Onde usar
 Essa metodologia pode ser  utilizada principalmente na criação de sistema de design web.
 Uma boa maneira de como utilizar a metodologia Atomic Design é escrever um bom CSS como mostra o exemplo a seguir. Desta maneira sugere-se que denomine os componentes menores e aplique os estilos a eles. Segundo Brad Frost, ele recomenda que seja criado um arquivo separado para cada elemento.
 ```html	
 		 / * ----------- Elementos globais (átomos) ------------ * /
		@import "headings";
		@import "links";
		@import "lists";
		@import "text";
		@import "buttons";
		 
		/ * ----------- COMPONENTES (Moléculas) ------------ * / 
		@import "forms";
		@import "pagination";
		@import "article";
		 
		/ * ----------- Content / Blocks (organismo) ------------ * / 
		@import "header";
		@import "footer";
		@import "menu";
		 
		/*----------- PAGE STRUCTURE (Templates) ------------*/
		@import "layout";
```		 
</br>
####Exemplos de cada Etapa
  Para exemplificar melhor cada etapa desta metodologia, segue abaixo imagens e trechos de códigos fontes.
</br>
#####Átomos
######Exemplo em imagem:
<img src="http://habaneroconsulting.com/~/media/hab/insights/2014/what-is-atomic-design/2014-07-14%202-19-14%20pm.ashx?la=en&hash=8E134410619BEFFE6B8966FABBD8078D5F2E3783">
######Exemplo em código fonte:
```html	
	<label>Código:</label>
	<input type="text" id="inputCod" name="inputCod">
```	
</br>
#####Moléculas
######Exemplo em imagem:
<img src="http://habaneroconsulting.com/~/media/hab/insights/2014/what-is-atomic-design/2014-07-14%202-18-55%20pm.ashx?la=en&hash=082A830F516D83F3231D49734A0B3F5BEEB909D0">
######Exemplo em código fonte:
```html		
	<form>
	    <label>Código:</label>
	    <input type="text" name="codigo" value="" placeholder="Informe o código">
	    <input type="submit" name="enviar" value="Enviar">
	</form>
```
</br>
#####Organismos
######Exemplo em imagem:
<img src="http://habaneroconsulting.com/~/media/hab/insights/2014/what-is-atomic-design/2014-07-14%202-18-30%20pm.ashx?la=en&hash=9B86E4E01E63346C27BAADC18D7C405C601A9223">
######Exemplo em código fonte:
```html	
   <header>
    <img src="logomarca.jpg">
    <nav>
        <ul>
            <li><a href="" title="Home"></a></li>
            <li><a href="" title="Community"></a></li>
            <li><a href="" title="Our Company"></a></li>
        </ul>
    </nav>    
	</header>
```
</br>
#####Modelos
######Exemplo em imagem:
<img src="http://habaneroconsulting.com/~/media/hab/insights/2014/what-is-atomic-design/2014-07-14%202-17-48%20pm.ashx?la=en&h=833&w=1192&hash=93E04473FFA985F833ABBAB7B96F204C34C88F39">
</br>
#####Páginas
######Exemplo em imagem:
<img src="http://habaneroconsulting.com/~/media/hab/insights/2014/what-is-atomic-design/2014-07-14%202-10-35%20pm.ashx?la=en&hash=7CDD0C658EC94716BFC207133435715A302931A6">
</br>
####Referências: 
http://bradfrost.com/blog/post/atomic-web-design/
http://tableless.com.br/o-que-e-design-atomic/
http://www.frontendbrasil.com.br/tutoriais/atomic-design-como-funciona/
http://nomadev.com.br/atomic-design-por-que-usar/
http://patternlab.io/about.html
http://habaneroconsulting.com/insights/what-is-atomic-design#.VilQCm7y33B
