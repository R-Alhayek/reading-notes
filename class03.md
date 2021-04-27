# Html: Lists
###### HTML provides us with three different types:
+ **Ordered lists**: are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order.
   + The ordered list is created with the (ol) element.
   **(li)**:Each item in the list is placed between an opening (li) tag and a closing (/li) tag. (The li stands for list item.)
+ **Unordered lists**: are lists that begin with a bullet point (rather than characters that indicate order).
   + The unordered list is created with the (ul) element.
   **(li)**:Each item in the list is placed between an opening (li) tag and a closing (/li) tag. (The li stands for list item.)
+ **Definition lists**: are made up of a set of terms along with the definitions for each of those terms.
   + The definition list is created with the (di) element and usually consists of a series of terms and their definitions. Inside the (di) element you will usually see pairs of (dt) and (dd) elements.
   **(dt)**: This is used to contain the term being defined (the definition term).
   **(dd)**: This is used to contain the definition.
   ![image](https://media.gcflearnfree.org/content/5e46ef60397c182fec255f32_02_14_2020/lists.png)

+ **Nested Lists**: You can put a second list inside an (li)element to create a sublist or nested list.   

# Css:Boxex
###### CSS treats each HTML element as if it lives in its own box. You can set several properties that affect the appearance of these boxes.
+ **Box Dimenitions**: 
  + **width, height**: By default a box is sized just big enough to hold its contents. The most popular ways to specify the size of a box are to use pixels, percentages, or ems.
    + **Limiting Width: min-width, max-width**: the
    min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.
    + **Limitting hight:min-height, max-height**: Sometimes you want to limit the height of it. This is achieved using the min-height and max-height properties.
+ **Overflowing Content: overflow**: The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
    + **hidden**: This property simply hides any extra content that does not fit in the box.
    + **scroll**: This property adds a scrollbar to the box so that users can scroll to see the missing content.
+ **Border, Margin & Padding**: Every box has three available properties that can be adjusted to control its appearance:
    + **Border**: Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.
    + **Margin**: Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
    + **Padding**: Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.
    + **border-width**: The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of thefollowing values: thin, medium, thick.
    + **border-style**: You can control the style of a border using the border-style property. This property can take the following values: solid, dotted, dashed, double, groove, ridge, inset, outset, hidden / none.
    + **border-color**: You can specify the color of a border using either RGB values, hex codes or CSS color names.
+ **Centering Content**: If you want to center a box on the page (or center it inside the element that it sits in), you can set the left-margin and right-margin to auto.
+ **Changing Inline/Block: display**: The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page.
![image](https://www.pngkit.com/png/full/110-1102927_enter-image-description-here-css-box-model-border.png)

# CSS3
+ **border-image**: The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces.
+ **box-shadow**: The box-shadow property allows you to add a drop shadow around a box.
+ **Rounded Corners**: CSS3 introduces the ability to create rounded corners on any box, using a property called border-radius. The value indicates the size of the radius in pixels.
+ **Elliptical Shapes**: To create more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners. For example, this will create a radius that is wider than it is tall: border-radius: 80px 50px;
![image](https://i.ytimg.com/vi/vn41-lpnjNM/maxresdefault.jpg)

