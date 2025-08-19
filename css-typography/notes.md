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

/* em - Relative to parent element 1em = 100% */
/* rem - Relative to the root (html ( font-size 16px) 1rem = 16px */
/* vw, vh --> Relative to viewport width and height */