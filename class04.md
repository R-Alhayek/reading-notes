# Html: Links
###### Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing. Links are created using the (a) element. Users can click on anything between the opening (a) tag and the closing (/a) tag. You specify which page you want to link to using the href attribute.
**(a href="http://www.imdb.com">IMDB</a)**
+ **Linking to Other Sites**: Users can click on anything that appears between the opening (a) tag and the closing (/a) tag and will be taken to the page specified in the href attribute. When you link to a different website, the value of the href attribute will be the full web address for the site, which is known as an absolute URL. Browsers show links in blue with an underline by default.
+ **Linking to Other Pages on the Sa me Site**: When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL.
   + **Same Folder**:  If all the pages of the site are in the same folder, then the value of the href attribute is just the name of the file. (a href="reviews.html">Reviews</a)
   + **Child Folder**: For a child folder, use the name of the child folder, followed by a forward slash, then the file name. (a href="music/listings.html">Listings</a)
   + **Parent Folder**: Use ../ to indicate the folder above the current one, then follow it with the file name. (a href="../index.html">Home</a).

+ **Email Links**: mailto: email-links.html HTML To create a link that starts up the user's email program and addresses an email to a specified email address, you use the (a)element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.
+ **Opening Links in a New Window**: target: If you want a link to open in a new window, you can use the target attribute on the opening (a) tag. The value of this attribute should be _blank.
+ **Linking to a Specific Part of the Same Page**: Before you can link to a specific part of a page, you need to identify the points in the page that the link will go to. You do this using the id attribute (which can be used on every HTML element).
+ **Linking to a Specific Part of Another Page**: As long as the page you are linking to has id attributes that identify specific parts of the page, you can simply add the same syntax to the end of the link for that page. Therefore, the href attribute will contain the address for the page (either an absolute URL or a relative URL), followed by the # symbol, followed by the value of the id attribute that is used on the element you are linking to.
![image](https://weblog.west-wind.com/images/2019/Non-Navigating-Links-for-JavaScript-Handling/EmptyHref.png)

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

# CSS Frameworks
###### CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.

#### The 960.GS CSS Framework:
###### 960.gs provides a style sheet that you can include in your HTML pages. Once our page links to this style sheet, you can provide the appropriate classes to your HTML code and it will create multiple column layouts for you.




