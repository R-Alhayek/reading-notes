# HTML: Images
###### Controlling the size and alignment of your images using CSS keeps rules that affect the presentation of your page in the CSS and out of the HTML markup.
![image](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2020/07/html-images-df.jpg)

#### Controlling sizes of images in CSS:
###### Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download. You might think that your site is likely to have images of all different sizes, but a lot of sites use the same sized image across many of their pages.

#### AligNing images Using CSS:
###### Rather than using the (img) element's align attribute, web page authors are increasingly using the float property to align images. There are two ways that this is commonly achieved:
+ **1: The float property**  is added to the class that was created to represent the size of the image.
+ **2: New classes** are created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image.

#### Centering images Using CSS:
###### By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a blocklevel element using the display property with a value of block. Once it has been made into a block-level element, there are two common ways in which you can horizontally center an image:
+ **1: On the containing element, you can use the text-align property with a value of center.**
+ **2: On the image itself, you can use the use the margin property and set the values of the left and right margins to auto.**

#### Background Images
###### The **background-image** property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box. The path to the image follows the letters url, and it is put inside parentheses and quotes.

#### Repeating Images: background-repeat / background-attachment
###### The background-repeat property can have four values:
+ **repeat** The background image is repeated both horizontally and vertically (the default way it is shown if the backgroundrepeat property isn't used).
+ **repeat-x** The image is repeated horizontally only.
+ **repeat-y** The image is repeated vertically only.
+ **no-repeat** The image is only shown once.

###### The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:
+ **fixed** The background image stays in the same position on the page.
+ **scroll** The background image moves up and down as the user scrolls up and down the page.

#### Background Position: background-position
###### When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed. This property usually has a pair of values. The first represents the horizontal position and the second represents the vertical. If you only specify one value, the second value will default to center.

#### shorthand: background
###### The background property acts like a shorthand for all of the other background properties you have just seen, and also the background-color property. The properties must be specified in the following order, but you can miss any value if you do not want to specify it.
**1: background-color
2: background-image
3: background-repeat
4: background-attachment
5: background-position**
![image](https://qph.fs.quoracdn.net/main-qimg-ef8eb5e0787252f9f5fad5e0dd1d63f6)

### Contrast of background images
###### If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible.
+ **High Contrast**: The majority of photographs have quite a high contrast, which means that they are not ideal for use as a background image.
+ **Low Contrast**: Image editing applications such as Photoshop and GIMP have tools that allow you to manually adjust your images to have lower contrast.
+ **Screen**: To overlay text on an image with high contrast, you can place a semi-transparent background color (or "screen") behind the text to improve legibility.
![image](https://i.stack.imgur.com/lUIR6.png)

# HTML: Practical Information
### Search Engine Optimization (SEO )
#### +The Basics
Search engine optimization (or SEO) is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers. In order to determine who comes first in the search results, search engines do not only look at what appears on your site. They also consider how many sites link to you (and how relevant those links are). For this reason, SEO is often split into two areas: on-page techniques and off-page techniques.

#### On-Page Techniques
The main component of this is looking at keywords that people are likely to enter into a search engine if they wanted to find your site, and then including these in the text and HTML code for your site in order to help the search engines know that your site covers these topics.
**In every page of your website there are seven key places where keywords can appear in order to improve its findability:**
**1: Page Title**
**2: URL / Web Address**
**3: Headings**
**4: Text**
**5: Link Text**
**6: Image Alt Text**
**7: Page Descriptions**


#### Off-Page Techniques
Getting other sites to link to you is just as important as on-page techniques. Search engines help determine how to rank your site by looking at the number of other sites that link to yours. They are particularly interested in sites whose content is related to yours. 

### How to Identify Keywords and Phrases:
###### Determining which keywords to use on your site can be one of the hardest tasks when you start to think about SEO. Here are six steps that will help you identify the right keywords and phrases for your site.
**1: Brainstorm:** List down the words that someone might type into Google to find your site. Be sure to include the various topics, products or services your site is about.
**2: Organize:** Group the keywords into separate lists for the different sections or categories of your website.
**3: Research:** There are several tools that let you enter your keywords and then they will suggest additional keywords you might like to consider, such as: adwords.google.co.uk/ select/KeywordToolExternal.
**4: Compare:** It is very unlikely that your site will appear at the top of the search results for every keyword. This is especially true for topics where there is a lot of competition. The more sites out there that have already been optimized for a given keyword, the harder it will be for you to rise up the search results when people search on that term.
**5: Refine:** Now you need to pick which keywords you will focus on. These should always be the ones that are most relevant to each section of your site.
**6: Map:** Now that you have a refined list of keywords, you know which have the most competition, and which ones are most relevant, it is time to start picking which keywords you will use for each page. Pick 3-5 keywords or phrases that map to each page of your website and use these as the keywords for each page.
![image](https://mk0apibacklinkov1r5n.kinstacdn.com/app/uploads/2019/08/google-still-scans-key-areas-of-your-site-1.png)

### Analytics: Learning about your Visitors
###### As soon as people start coming to your site, you can start analyzing how they found it, what they were looking at and at what point they are leaving. One of the best tools for doing this is a free service offered by Google called Google Analytics.

### How Many People Are Coming to Your Site?
###### The overview page gives you a snapshot of the key information you are likely to want to know. In particular, it tells you how many people are coming to your site.

### What Are Your Visitors Looking At?
###### The content link on the left-hand side allows you to learn more about what the visitors are looking at when they come to your site.

### Where Are Your Visitors Coming From?
###### The traffic sources link on the left hand side allows you to learn where your visitors are coming from.

### Domain Names & Hosting



