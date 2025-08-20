# Colors and Background 
- colors and backgrounds play a major role in web design. They help create branding readablility and user experinces 

- Text and color : color theory 
- Background images and gradiants 
- Background positioning and sizing 
- Background transparency 

# Color

< style>

        .red {
          color: red;
        }

        .blue {
           color: blue;
        }

        .custom {
            color: #ff6600;

        }

< body>

    <p class="red">This is red text</p>
    <p class="blue">this is blue text</p>
    <p class="custom">this is custom text</p>

# Background 

Example:

< style>

        .bg-light {
            background-color: lightgray;
            padding: 20px;
        }

        .bg-dark {
            background-color: black;
            color: white;
            padding: 20px;
        }
  
< body>

    <div class="bg-light"> light Background</div>
    <div class="bg-dark"> dark Background</div>

# Background Images

< style >

 .bg-image {
            background-image: url("Background.jpg");
            height: 200px;
            background-size: cover;
            background-position: center;
        }

  < body>      

    <div class="bg-image">Background images</div>

# Background positioning 
use background positioning to align images
- values 
  - left top: aligns to the top left
  - center center: aligns to the center
  - right botto: aligns to the bottom right
  

  < style>

         .bg-image {
           background-image: url("Background.jpg");
           background-position: center center;
           height: 500px;
        }

< body>        

     <div class="bg-image">Background images</div>

# Background sizing 
defines how an image fits within and element 
- values 
 - auto 
 - cover: will fill the space
 - contain: keeps it fully visible

 < style>

   .bg-image {
           background-image: url("Background.jpg");
           background-position: center center;
           height: 500px;
        }
         
        .bg-cover {
            background-size: cover;
        }

        .bg-contain {
            background-size: contain;
        }

< body>     

     <div class="bg-image bg-cover">Background images</div>
                          or 
     <div class="bg-image bg-contain">Background images</div> 

- contain sometimes causes image tiling in effor to fit by what it can for example in the rectangular shape it will try to fit and create a repetative image.

# Backgound Repeating
Controls image tiling 
- values 
 - repeat: repeats in both directions
 - repeat X: repeats horizontally 
 - repeat y: repeates vertically
 - no repeat: no repetiton 


    .bg-no-repeat {
            background-repeat: no-repeat;
        }

        .bg-repeat {
            background-repeat: repeat;
        }

 - use no repeat for unwanted tiling and repeate is the default

 # Background attachemnt 
 controls wheather the background images scroll with the webpage. Background attachments in CSS have
 - Values 
  - Scroll: moves with page scroll
  - fixed: stays in one place
  - local: moves within the elements context

  .bg-fixed {
            background-attachment: fixed;
        }
  
# Background gradiants
Gradiants are smooth color transitions the background has linear gradiant and there are different types linear and radial gradiant. gradiants improve modern design aesthetics

linear: is left to right 
radial: is like a cricle

.gradiant {
            background: linear-gradient(to right,red,blue);
        }


.gradiant {
            background: radial-gradient(circle,red,blue);
        }






