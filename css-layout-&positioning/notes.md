# CSS Layout & Positioning 
Define how elements are arranged on a webpage
- Display properties (block,inline,flex grid)
- Positioning and spacing (static,relative,absolute,fixed,sticky)
- Alignment and spacing (top,right,bottom,left z-index)
- Overflow handling 

# Display
the display property defines how an element behaves in the layout.
(block,inline,flex,grid)
- # Block: 
block starts on a new line, takes full width. Examples that have dfault block are div, p, h1, and section
- # Inline: 
inline only take needed width. Examples of default inline are span, a, and strong.

Block element stack and inline elements stay in the same line.

Example:

< style>

    .block {
        background-color: lightblue;
        padding: 10px;
    }

    .inline {

        background-color: lightgreen;
        padding: 5px;
    }

< body>

    <div class="block">i am a block element</div>
    <span class="inline">i am inline</span>
    <span class="inline">i am inline too</span>   

- You can change the default values  
for the span tags were changing the display: to block so that they stack 
and for the div we are changing the display: to inline so the go side by side.

Example:

  span {
        display: block;
        width: 200px;
     }

     div {

        display: inline;
     }

  < body>

    <div class="block">i am a block element</div>
    <div>div acting like span</div>
    <span class="inline">i am inline</span>
    <span class="inline">i am inline too</span>     

- adding a hidden class - will cause the element to dissapear if you add the .hidden class to the div

Example:

      span {

        display: block;
        width: 200px;
     }

     div {

        display: inline;
     }

     .hidden {

        display: none;
     }

< body>

    <div class="block">i am a block element</div>
    <div class="hidden">div acting like span</div>
    <span class="inline">i am inline</span>
    <span class="inline">i am inline too</span>


# Positioning 
The position property determines how elements are placed on a page 
Position types:
- # Static
(default) | Normal flow, no positioning

Example:

< style>

    .static {
        position: static;
    }

< body>

    <p class="static">i am static</p>  

- # Relative
Moves relative to its normal position

Example:

< style>

    .static {
        position: static;
    }

    .relative { 
        position: relative;
        top: 20px;
        left: 30px;
    }

< body>

    <p class="static">i am static</p>
    <div class="relative">i am relative</div>


- # Absolute
Moves relative to the nearest positioned ancestor

Example: 

< style>

         .parent {
        position: relative;
        width: 300px;
        height: 200px;
        background-color: lightgrey;
     }

     .absolute {
        position: absolute;
        top: 20px;
        left: 50px;
        background-color: lightcoral;
     }

< body>     

      <div class="parent">
        <div class="absolute">i am absolute</div>
    </div>

- the absolute positons itself inside the parent 

- # Fixed
Stays fixed on the screen no matter where you go to on the page

Example:

< style>

    .fixed {
        position: fixed;
        bottom: 10px;
        right: 10px;
        background-color: yellow;
     }

 < body>

     <div class="fixed">i am fixed</div>    

- # Sticky
Sticks when scrolling past a point



