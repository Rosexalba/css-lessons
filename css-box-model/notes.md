# Box Model 
The css box model determines how elements take up space on a webpage 
every HTML element is a rectangular box with four layers.
- Content: which is the text, image, or other content inside the element
- Padding: which is the space between the content and the border
- Border: which is the edge around the element.
- Margin: Whis is the space outside the element. Seperating it from others.


Example: 

< style>

   .box {

            width: 200px;
            height: 100px;
            padding: 20px;
            border: 5px solid black;
            margin: 30px;
            background-color: lightblue;
        }

< body>

    <div class="box">Hello, I'm a box!</div>


# Width & Height:
By default width and height only affects the content area 

Example: 

< style>

      .box {
        
            width: 250px;
            height: 150px;
            background-color: lightgray;
        }

- Problem : the actual size of the element will be larger if padding and border are added.     

# Padding:
The space between the content and the border 
- padding goes in a clockwise format which is top,right,bottom,left.

Example:

< style>

    .box {
            padding: 10px 20px 15px 5px;
    }

# Border & Margin
- Border: wraps around the content and padding (the edge around the element)
it can be written in short hand or long hand. Width -> style -> color

short hand:

.box {

            border: 5px solid black;

long hand: 

.box {

            border-width: 5px;
            border-style: solid;
            border-color: black; 

 - if you want rounded border    

            border-radius: 15px;      

 - square into circle

 .box {

            border: 1px solid black;
            height: 100px;
            width: 100px;
            border-radius: 50px;    

# Margin 
Creates space outside the border creating space. margin is also in clockwise top,right,bottom,left. width -> style -> color


- shorthand:

    .box {

       margin: 30px 10px 5px 30px;    

- auto centering: center is a block element horiztonally

        width: 200px;
        background-color: lightblue;
        margin:auto

# Box-sizing
to fix box sizing issues by default width and height exclude padding and border making the actual size larger 

.box {

            width: 200px;
            height: 100px;
            padding: 20px;
            border: 5px solid black;

- the problem here is that now the box size is bigger than 200 pixels by 100 pixels.

The solution is adding box-sizing: border-box;

.box { 
              
            width: 200px;
            height: 100px;
            padding: 20px;
            border: 5px solid black;
            box-sizing: border-box;

 now width and heigh include padding and border keeping the box size fixed.

# Box shadow 
this is adding depth create a 3d effect around an element

.box {

          box-shadow: 5px 5px 10px black;

- shorthand:

box-shadow: x-offset -->  y-offset -->  blur-radius -->  color          




       

