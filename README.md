# Guia-CSS

this is the first page i've done while studying for css style tools.

CSS is a tool for optimize the style of your website. As we can see in the style.css, file we need to put some attributes for each sector that we call in our html file.

for example.

We have a tag called h1, which means the first heading tag, in this css file, we put an "{}" in front of this element to put the attributes inside of it, theres a lot of attributes we can put in each tag of our html file and the css will help us to style this elements. 
    
    h1{
      text-align: center;
      font-size: 60px;
      }

In another example we have the "*" tag that we can put some attributes too, this "*" tag is a tag for the all page, would be very usefull to put the "font-family" on this tag because the all page is using the same font.

    *{
      font-size: 10px; /* px significa "pixels": o tamanho da fonte base é agora de 10 pixels */ 
      font-family: "Open Sans", sans-serif; /* este deve ser o nome da fonte que você obteve no Google Fonts */ 
     }

Today i am very grateful to learn all about the 'position' tool in css, with this tool you can make for example a menu that overlaps the top of the page, or the position you prefer, until the end of it. With just this you can make your design very responsive and helpful for the user.
    html
    
    .menu-fixed{
	    width: 100%;
	    height:200px;
	    background: #069;
	    position: fixed; /* o item em questão fica fixo na tela até o final da página*/

    }	
    .box{
	    width: 100%;
        height: 1400px;
	    background:green;
    }
    
In this example we can see an div that correspond with a menu that overlaps the rest of the page, in this case the menu is always there in case you wanna go somewhere else.

BACKGROUND
In this lesson we will know all about background in css
example

	.bg{
		background-color: #ccc;
		background-color: rgba(200, 200, 200, 0.4); 
		background-color: gray;

	}
In the first case, there's the hexadecimal code for the color.
In this seconde case, the rgba it means the 3 shades of red, green and blue and the opacity.
In the last case, we just put the name of the color you want.

You can put an image in your website being imported by the css like this.
	
	.bg{
		background-image:url('../imagens/imagem.jpg')
	}


