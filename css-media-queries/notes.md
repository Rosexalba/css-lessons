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
 - Typography
 - Layouts
 - Images

 # Mobile-first 
 
 # Desktop-first Design
