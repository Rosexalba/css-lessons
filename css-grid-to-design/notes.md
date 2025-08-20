# CSS Grid
css grif is a powerful layout sytem that allows you to design two dimensial layouts with rows and columns. It is more flexible than flexbox when working with complex page layouts 


- What is Css Grid & why use it?
css grid is a 2 dimensional system the allows items to be postioned in rows and columns. Css grid creates complex layouts easily, better for structuring full web pages, precise control over placement.

# Enable grid  
(display:grid)
to enable css grid set css grid with diplay grid. set display grid on a parent container 

 < style>

        .grid-container {
            display: grid;
            background-color: beige;
            padding: 10px;
        }

< body>      

   < div class="grid-container">

    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>

   < /div>  

- Items are stacked virtically by default on grid.

# Defining columns & rows 
Use
- grid-template-columns 
- grid-template-rows 
to create a structured grid 

< style>

 .grid-container {
            display: grid;
            background-color: beige;
            padding: 10px;
            grid-template-columns: 100px 100px 100px ;
            grid-template-rows: 100px 100px;
        }

 - this grid is creating three columns and two rows  

 # FR 
 using FR (flexible fraction) instead of pixels use FR for dynamic resizing. so in the grid template columns instead of 100 pixels 
 you will use 1fr 2fr 3fr 

 - grid-template-columns: 1fr 2fr 1fr ;

# Placing Items in the grid 
use
- grid-column 
- grid-row 
to position elements

< style>

     .item:nth-child(1) {
            grid-column: span 2;
            grid-row: span 2;
        }

- the first item now spans two columns and two rows

# spacing 
- grid gaps: use gap to add space between grid items
gap:20px
- adds even spacing between all grid items 

# aligning items

- justify items horizontal alignment 
    - start: aligns to left
    - center: aligns to center 
    - End: aligns to the right

    justify-items: start;

- Align itmes vertical alignment
    - start: top
    - center: center
    - end: bottom

     align-items: end;

- place items shorthand combine
This will center both items both horizontally and vertically. its combines justift items and align items 

     place-items: center;
 



# advanced grid-features 
- grid-template-areas :define a named layout 

< style>

        .grid-container {
            display: grid;
            grid-template-columns: 200px 1fr;
            grid-template-rows: 80px 1fr 60px;
            grid-template-areas: 
            "header header"
            "sidebar content"
            "footer footer"
        }

        .header {
             grid-area: header; background-color: lightblue;
        }

        .sidebar {
            grid-area: sidebar; background-color: lightgray;
        }

        .content { 
            grid-area: content; background: white
        }

        .footer { 
            grid-area: footer; background-color: lightgreen;}


< body>

    <div class="grid-container">
        <header class="header">Header</header>
        <aside class="sidebar">Sidebar</aside>
        <main class="content">content</main>
        <footer class="footer">Footer</footer>
    </div>



