# Typography
Typography is one of the most important aspects of web design. it determines how a text looks feels and behaves on a webpage.

- Font family (choosin the right font)
- Font size (scaling tex appropriately)
- Font weight & style (bold,italic, etc.)
- Text alignment & spacing (line height, letter spacing)
- Text transformation & decoration ( uppercase,underline, etc.)
- Google fonts (importing custom fonts)

# Font size 


  < style>
       
        .small {
            font-size: 12px;
        }
        .medium {
            font-size: 18px;
        }
        .large {
            font-size: 24px;
        }

        .relative-size {
            font-size: 1.5em;
        }

        .viewport-size {
            font-size: 5vw;
        }


< body>

    <p class="small">this is small text</p>
    <p class="medium">this is medium text</p>
    <p class="large">this is large text</p>
    <p class="relative-size">this is relative-size</p>
    <p class="viewport-size">Viewport size</p>

# values

- em - Relative to parent element 1em = 100% 
- rem - Relative to the root ( html ( font-size 16px) 1rem = 16px 
- vw, vh --> Relative to viewport width and height 

# Font Weight & Font style
font weight refers to the boldness of text and font style refers italics or normal.

< style>

        .light {
            font-weight: 300;

        }

        .normal {
             font-weight: 400;
        }

        .bold {
             font-weight: 700;
        }

< body>

    <p class="light">light text</p>
    <p class="normal">medium text</p>
    <p class="bold">bold text</p>


- values range from 100 to 900 

- font style 

< style>

      .italic {
            font-style: italic;
        }

< body>

      <p class="bold italic">bold text</p>


# Text Alignment
The text alignment property controls horizontal text placement

 < style>

        .left {
            text-align: left;
        }

        .center {
            text-align: center;
        }

        .right {
            text-align: right;
        }

< body>

    <p class="left">left aligned</p>
    <p class="center">center aligned</p>
    <p class="right">right aligned</p>

# line height and spacing 
controls the space between lines
- Letter spacing and word 

< style>

 .spacing {
            line-height: 5; 
        }

        .letter-spacing {
            letter-spacing: 10px;
        }

        .word-spacing { 
            word-spacing: 50px;
        }

# Text-transformation and Decoration  


 < style>

        .uppercase {
            text-transform: uppercase;
        }

        .lowercase {
            text-transform: lowercase;
        }

        .capitalize {
            text-transform: capitalize;
        }

        .underline { 
            text-decoration: underline;
        }

        .line-through {
            text-decoration: line-through;
        }

        .no-decoration {
            text-decoration: none;
        }

< body>

    <p class="uppercase underline">uppercase</p>
    <p class="lowercase line-through">LOWERCASE</p>
    <P class="capitalize">capitalize</P>
    <a class="no-decoration" href="https://google.com">google.com</a>
   
# Importing google fonts 
- HTML has great fonts built in but sometimes we want different style or mor variety in custom fonts.
- Head over to the google font webpage 
fonts.google.com
- There you click 'Get font' after you see one you like this will give you the code to link to your page and the css code for styling 


