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

By default in case the width and height pass the size of the image it will be continued below, so that it doesn't happen there is the following property that will adjust the image just for it own size.	
	
	background-repeat: no-repeat;
	
<blockquote>it is completely possible to do the opposite with the 'repeat-x' and 'repeat-y' attributes AND changing the 'background-size' to test the better way to make use of your background image</blockquote>

The CSS background-size property specifies the size of the background images. The size of the image can be totally or only partially in order to preserve its aspect ratio.	
	
	background-size: cover;

#CSS3 Flexbox: Functioning and properties
        
The flexbox is a CSS3 concept that aims to organize the elements of an html page inside his own containers in a dinamic way. That is, independent of his own dimensions they always maintain a flexible layout inside his father element, reorganizing itself and according to the needs of.

	html
	<div class="container">
	     <div class="item item1"></div>
	     <div class="item item2"></div>
	     <div class="item item3"></div>
	 </div>

css
<h2>display</h2>

	.container{
	    display:flex;
	}

This is necessary for the other properties to show the expected result.

The flex-direction property must be applied to the container and defines the display axis / flow in which the elements will be organized.

	.container{
	    display:flex;
	    flex-direction:[row / row-reverse / column / column-reverse];
	}	
   "row" (default): The items are organized inline from the left to right 
   "row-reverse": The items are organized inline from the right to the left
   "column":  The items are organized in columns starting from the top to the bottom
   "column-reverse": The items are organized in columns starting from the bottom to the top
        

	.container {
	     display: flex;
	     flex-wrap: [nowrap / wrap / wrap-reverse]; 
	}
"nowrap" (default): All items are disposed in one line;
"wrap": The line will break and the rightmost items will be moved to the bottom line;
"wrap-reverse": The line will break and the rightmost items will be moved to the top line;


<h2>Flex-flow</h2>
This property is a short form for writing the flex-direction and flex-wrap properties, in that order. Therefore, it applies to the container.

Usually these properties are defined one by one, as follows:

	.container {
	    display: flex;
	    flex-direction: column;
	    flex-wrap: wrap;
	}

With flex-flow we can write both in a simplified way:
    flex-flow: column wrap;

<h2>justify-content</h2>
The justify-content property defines the alignment of items along the main axis of the container. The syntax and possible values ​​for this property are shown below:
	
	.container {
	     display: flex;
	     justify-content: [flex-start/flex-end/center/space-between/space-around];
	}
"flex-start" (default): Items are aligned from the beginning of the main axis;
"flex-end": Items are aligned from the end of the main axis;
"center": Items are aligned to the center of the main axis;
"space-between": The first item is moved to the beginning of the main axis, the last is moved to the end of the main axis and the rest are evenly distributed among them;
"space-around": Items are evenly distributed along the main axis. Here, however, equal margins are assigned to the left and right (or up and down, depending on the direction of the main axis). For this reason, the first and last items are not “glued” to the edges of the container.

<h2>align-content</h2>

This property defines how the lines are distributed along the container's transversal axis. The syntax and possible values for this property are shown below:
	
	.container {
	    display: flex;
	    align-content: [stretch/flex-start/flex-end/center/space-between/space-around];
	}
    
"stretch" (standard): The lines are evenly distributed along the transversal axis, occupying all the available space;
"flex-start": The lines are distributed from the beginning of the transversal axis;
"flex-end": The lines are distributed from the end of the transversal axis;
"center": The lines are kept in the center of the transversal axis;
"space-between": The first line is shifted to the beginning of the transverse axis, the last is shifted to the end of the transverse axis and the rest are evenly distributed between them;
"space-around": The lines are evenly distributed along the transverse axis. Here, however, equal margins are assigned to the left and right (or above and below, depending on the direction of the transverse axis). That is why the first and last lines are not “glued” to the edges of the container.

<h2>align-items</h2>
This property defines how the items are distributed along the transversal axis of the container. The syntax and possible values for this property are shown below:
	
	.container {
	    display: flex;
	    align-items: [stretch/flex-start/flex-end/center/space-between/space-around];
	}

"stretch" (default): Items will be stretched to fill the entire dimension of the transverse axis (height or width);
"flex-start": Items are moved to the beginning of the transversal axis;
"flex-end": Items are moved to the end of the transverse axis;
"center": Items are centered on the transversal axis;
"baseline": Items are aligned from the bottom of the first line of text for each.

