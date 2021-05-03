# CSS:Layout
###### we are going to look at how to control where each element sits on a page and how to create attractive page layouts. 
#### Key Concepts in Positioning Elements:
+ **Building Blocks**: CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
   + **Block-level elements** start on a new line Examples include: (h1) (p) (ul) (li).
   + **Inline elements** flow in between surrounding text Examples include: (img) (b) (i).
+ **Containing Elements**: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
#### Controlling the Position of Elements:
+ **Normal flow**: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. Even if you specify the width of the boxes and there is space for two elements to sit side-byside, they will not appear next to each other. This is the default behavior. the syntax would be:
position: static;
+ **Relative Positioning**: This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow.
You can indicate that an element should be relatively positioned using the position property with a value of relative.
+ **Absolute positioning**: This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page. When the position property
is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page. (They act like it is not there.)
    + **Fixed Positioning**: Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed. It positions the element in relation to the browser window. Therefore, when a user scrolls down the page, it stays in the exact same place.

+ **Floating Elements: float**: The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. Anything else that sits inside the containing element will flow around the element that is floated. 
     + **USING Float to Place Elements Side-by-Side**: A lot of layouts place boxes next to each other. The float property is commonly used to achieve this. When elements are floated, the height of the boxes can affect where the following elements sit.
     + **Clearing Floats: clear**: The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box.
     + **Creating Multi-Column Layouts with Floats**: The following three CSS properties are used to position the columns next to each other:
         + width: This sets the width of the columns.
         + float: This positions the columns next to each other.
         + margin: This creates a gap between the columns.
![image](https://i.ytimg.com/vi/lyM_2iVQ814/hqdefault.jpg)

# Screen Sizes
###### Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.
+ **Screen Resolution**: Resolution refers to the number of dots a screen shows per inch. It is interesting to note that the higher the resolution, the smaller the text appears.
+ **Page Sizes**: Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).
+ **Fixed Width Layouts**: Fixed width layout designs do not
change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels.
+ **Liquid Layouts**: Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

#Layout Grids
###### Grids set consistent proportions and spaces between items which helps to create a professional looking design.
##### Possible Layouts:
+ **960 Pixel wide/12 Column Grid**: The page is 960 pixels wide and there are 12 equal sized columns , each of which is
is 60 pixels wide. Each column has a margin set to 10 pixels, which creates a gap of 20 pixels between each column and 10 pixels to the left and right-hand sides of the page.

# CSS Frameworks
###### CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.

#### The 960.GS CSS Framework:
###### 960.gs provides a style sheet that you can include in your HTML pages. Once our page links to this style sheet, you can provide the appropriate classes to your HTML code and it will create multiple column layouts for you.

#### Multiple Style Sheets: @import
##### There are two ways to add multiple style sheets to a page:
   + 1: Your HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets.
   + 2: In the HTML you can use a separate <link> element for each style sheet.


