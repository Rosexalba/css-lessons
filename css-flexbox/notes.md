# FlexBox 
Flexbox is a css layout model that allows elements to be easily aligned, spaced, and resized within a containe. It makes designing responsive layouts much easier.


main axis -------------->
                
                |
                |
                |
                |
                |
                |
           Cross axis 
 
 # What is flexbox and why use it?
 Flexbox layout is one-dimensional layout system that arranges elements horizontally in rows or vertically in columns. it makes it easier to align elements, centering, spacing, distributing, adapts to different screen sizes, great for responsive design, reduces the need foe floats and positioning hacks. 

 # how to enable flexbox with the css display flex property 
To activate flexbox set display flex on the parent container

< style>

        .flex-container {
            display: flex;
            background-color: lightgray;
            padding: 10px;
        }

        .item {
            background-color: steelblue;
            color: white;
            padding: 20px;
            margin: 5px;
        }
  
< body>

    <div class="flex-container">
        <div class="item"> Item 1</div>
        <div class="item"> Item 2</div>
        <div class="item"> Item 3</div>
    </div>

- tip:
div.item*3 will emmet and create three items

# Flex Direction
The flex direction property controls the main axis direction
 - row: is the default setting and goes left to right 
 - column: will cause the items to stack from top to bottom and take up as much space
 - row reverse: would reverse the row 
 - column reverse: items stacked from bottom to top 

< Style >

 .flex-container {
            display: flex;
            background-color: lightgray;
            padding: 10px;
            flex-direction: column;
 }
            

 - Aligning Items 
 - # justified content 
 - justified content: aligns on the main axis, controls horizontal alignment in a row
  - Values:  
    - flex-start (default left to right)
    - flex-end 
    - center 
    - space-around 
    - space-between
    - space-evenly 

< style>

.flex-container {
            display: flex;
            background-color: lightgray;
            padding: 10px;
            flex-direction: row;
            justified content: space-between 
}

# align-items 
- aligns on cross axis. controls vertical alignment on default 
 - Values:
    - Flex-start: puts items to the top 
    - flex-end: puts it to the bottom
    - center: middle
    - stretch: (default)
    - baseline: aligns text to the base line 

< style>

        .flex-container {
            display: flex;
            background-color: lightgray;
            padding: 10px;
            /* flex-direction: column; */
            justify-content: space-between;
            height: 200px;
            align-items: center;

# align-self
align-self overrides the alignment for a single item. it aligns and individual item differently. 

< style >

    .item:nth-child(2) {
            align-self: flex-end;
        }

- This will move item two to the bottom of the container. 

# Wrapping items (flex-wrap)
by default items stay in one row use flex box to wrap items when needed. 
flex-wrap: wrap - wraps items 
flex-wrap: nowrap - will try to stick everything in one line and it will over flow
flex-wrap: wrap-reverse- will wrap items in reverse

< style>

     .flex-container {
            display: flex;
            background-color: lightgray;
            padding: 10px;
            /* flex-direction: column; */
            justify-content: flex-start;
            height: 200px;
            align-items: baseline;
            flex-wrap: wrap-reverse; }

