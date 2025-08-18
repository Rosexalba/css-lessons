# Vocabulary
CSS Selectors: define which HTML elemens to style. They help target specific elements and apply styles effectively. This module covers basic selectors.
<br/>

# Basic selectors
- These selectors apply styles to elemeents based on tag names, classes, IDs and attributes.

# Universal Selector: 
- 'the star' targets all elements on the page.

  Example: the universal selector: in this example removes default margin padding from all elements and if wanted to you can change all text to a certain color

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-b9ox;
            color: purple;
        }

# Type: 
- targets elements by tag name 

  Example: Type selector targets elements by tag name in this example we will be using the h1 tag and the p tag to change the color font size of h1 and the color of the p tag
  
    < style>

       h1 {
        color: purple;
        font-size: 24px;
       }

       p {
        color: peru;
       }
    < / style>

# Class: 
- Class selector targets elements with a specific class

  Example: to grab all the class selector we did 
  .highlights next to get desired look we added a background-color of yellow to highlight and changed the font weight to bold.

        < style>

        .highlight {
            background-color: yellow;
            font-weight: bold;
        }

        < style>

        < body>

        <p class="highlight">paragraph</p>

        < body>

   classes can be reused across multiple elements     

# ID: 
- ID selector targets an element with a unique ID selector 

Example: to select ID you will use a #. Here we added color and changed the font size to 20px

< style>

    #uniqueText {
        color: red;
        font-size: 20px;
    }

< /style>

< body>

    <p id="uniqueText">Hello World</p>

Use ID sparsely, each ID should be unique. 


# attribute: 
- The attribute selector targets elements based on attributes and values 

Example: for attribute selector you will use the input tag with a style type.
Here you will be using [] after input with type inside the brackets to select. Only the < p> tag with type " text " will be styled. you will now have a solid blue border.

< style>

    input[type='text'] {
        border: 2px solid blue;
    }

< /style>

< body>

    <input type="text" placeholder="Enter your name" />
    <input type="passowrd" placeholder="Enter your password" />

Useful for styling forms and buttons 

<br/>

# Combinators
- Combinators target elements based on their relationship with other elements.


- Descendant: The descendant selector targets all matching elements inside another element

Example: here only the p tag inside the div will be styled in the color green
<!-- Desedant selector -->
 < style>

    div p {
        color: green;
    }

< /style>

< body>
<!-- Desendant selector -->
    < div>
        < p>this is inside a div< /p>
    < /div>
    < p>this is not a colored div< /p>
    
- Child: The child selector, parent to child targets direct children of an element.

Example: to select the child selector you will use >
<!-- Child selector -->
< style>

      div > p {
        color: blue;
    }

< /style>

< body>
<!-- Child selector -->
 < div>

        < p>direct child</p>
        < section>
            < p>not a direct child</p>
        < /section>
        
    < /div>


- Sibiling
<br/>

# Pseudo-classes
- :hover
- :focus
- :nth-child
<br/>

# pseudo-elemnts
- ::before
- ::after
   


 