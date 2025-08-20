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
        
 - Layouts
 - Images

 # Mobile-first 
 
 # Desktop-first Design
