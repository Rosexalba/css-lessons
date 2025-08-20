# Media queries
- responsive design makes websited adapt to different screen sizes
- media queries allow developers to apply CSS roles based on screen width/height or device type 


- What are media queries and why use them?
Media queries are a css feature that detects screen size and applys specific styles accordingly. insures a great user experience on all devices. avoids horizontal scrolling on screens and optimizes perfomances by loading correct styles.

# @media rules 
- changes background color based on the screen width 

# Breakpoints for different devices 

< style>

        body {
            font-family: arial, sans-serif;
            background-color: white;
            text-align: center;
            padding: 20px;
        }

        /* Tablet */
        @media (max-width: 768px){
            body {
                background-color: lightgray;
            }
        }

          
        /* Mobile */
        @media (max-width: 600px){
            body {
                background-color: hotpink;
            }
        }
       
# Responsive
 - Typography : changes size based on screen width 

     < style>

        body {
            font-family: arial, sans-serif;
            text-align: center;
        }

        /* Default size/ rem 3x times the size from the root*/
        h1 {
            font-size: 3rem;
        }

        /* Tablet */

        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }    
        }

        /* Mobile */
        @media (max-width: 480px) {
            h1 {
                font-size: 1.5rem;
            }
        }

 - Layouts: grid to stack column layout on small screens

 < style>

        body {
            font-family: Arial, sans-serif;
            text-align: center;
        }

        .container { 
            display: grid;
            grid-template-columns:  1fr 1fr 1fr;
            gap: 10px;
            padding: 20px;
        }

        .box {
            background-color: steelblue;
            color: white;
            padding:20px;
            text-align: center;
            border-radius: 5px;
        }

        @media (max-width:768pc) {
            .container {
                grid-template-columns: 1fr;
            }
        }

 < body>

    <div class="container">
        <div class="box">1</div>
        <div class="box">2</div>
        <div class="box">3</div>
    </div>



 - Images: Insures images resize properly on all screens 
 
 < style>

     body {
            font-family: Arial, Helvetica, sans-serif;
            text-align: center;
        }

        img { 
            max-width: 100%;
            height: auto;
            border-radius: 10px;
        }

< body>

    <h1>Responsive Images</h1>
    <img src="/home/rosexalba/css-lessons/css-colors-&backgrounds/Background.jpg" alt="">

- now you will be able to keep images from overflowing on small screens.

 # Mobile-first 
 
 # Desktop-first Design
