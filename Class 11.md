> # Class 11 *Jan 17 2021:*

> ## Topics

  1. Images
  
  2. Practical Information
  
  3. History of Flash 

---

> ## 1. Images

![Images](https://webmeup.com/upload/blog/lead-image-105.png)

---

####  **Controling Images Size in CSS:**

**You can control the size of an image by:**

  1. width
  
  2. Height
  
**Examples:**

      img.large {
         width: 500px;
         height: 500px;
         }
      img.medium {
         width: 250px;
         height: 250px;
         }
      img.small {
         width: 100px;
         height: 100px;
         } 

---

####  **Aligning images:**

**You can align an image by :**

  1. float: left & right
  
**Examples:**

    img.align-left {
      float: left;
      margin-right: 10px;
    }
    img.align-right {
      float: right;
      margin-left: 10px;
    }
    img.medium {
      width: 250px;
      height: 250px;
    }

---

#### **Centaring images:**

**By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image use:**
  
  1. `display:block`
  
  2. `margin: 0 auto`

**Examples:**

    img.align-center {
      display: block;
      margin: 0px auto;
      }
    img.medium {
      width: 250px;
      height: 250px;
      }

---

#### **Background images**    

**You can insert an image in a backgound by :**

  1. `background-image`: allows you to place an image behind any HTML  element. This could be the entire page or just part of the page. By  default, a background image will repeat to fill the entire box.
  
 
**Example:**

    background-image: url("images/pattern.gif");}
  
---

#### **Repeating Images:**    

  1. Repeating Images: it uses `background-repeat` with four different values
  
    1. repeat: The background image is repeated both horizontally and vertically
    
    2. repeat-x: The image is repeated horizontally only (as shown in the first example on the left). 
    
    3. repeat-y: The image is repeated vertically only.

    4. no-repeat: The image is only shown once. 
  
  2. `background-attachment`: specify it for the image to move or stays in its position. it takes two values:
  
    1. fixed: The background image stays in the same position on the page.
    
    2. scroll: The background image moves up and down as the user scrolls up and down the page.

**Examples:**

    background-image: url("images/tulip.gif");
    background-repeat: no-repeat;
    background-attachment: fixed;


----

#### **Background Position:**

**When an image is not being repeated, you can use the  `background-position`  property to specify where in the  browser window the background image should be placed with numaric values or these values :**

  1. `left top` 
  
  2. `left center`
  
  3. `left bottom`
  
  4. `center top`
   
  5. `center center`
  
  6. `center bottom`
  
  7. `right top`
  
  8. `right center`

  9. `right bottom`

    
**Examples:**


      body {
        background-image: url("images/tulip.gif");
        background-repeat: no-repeat;
        background-position: 50% 50%;
      }

----

#### **Images Rollover & Sprites**

**Using CSS, it is possible to create a link or button that changes to a  second style when a user moves  their mouse over it (known as a  rollover) and a third style when they click on it.**


**Examples:**

`<a class="button" id="add-to-basket"> Add to basket</a>` 

`<a class="button" id="framing-options"> Framing options</a> `


      `a.button {
          height: 36px;
          background-image: url("images/button-sprite.jpg");
          text-indent: -9999px;
          display: inline-block;
           }
      a#add-to-basket {
          width: 174px;
          background-position: 0px 0px;
           }
      a#framing-options {
          width: 210px;
          background-position: -175px 0px;
           }
      a#add-to-basket:hover {
          background-position: 0px -40px;
          }
      a#framing-options:hover {
          background-position: -175px -40px;
           }
      a#add-to-basket:active {
          background-position: 0px -80px;
          }
      a#framing-options:active {
          background-position: -175px -80px;
      }`

----

#### **CSS Gradients**

**CSS3 is going to introduce the ability to specify a gradient for the background of a box. The gradient is created using the background-image property and, at the time of writing, different browsers required a different syntax.**

**Examples:**

    background-image: -o-linear-gradient(#336666, #66cccc); 
    
---

> ## 2. Practical Information

![SEO](https://www.advotisa.com/wp-content/uploads/2019/05/image11-12.png)

#### **Search Engine Optimization (SEO)**

**SEO:** which is the practice of increasing the quantity and quality of traffic to your website through organic search engine results.

  1. The Basics: is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers.
    
  2. On-Page Techniques: On-page techniques are the methods you can use on your web pages to improve their rating in search engines.

     1. Page Title: The page title appears at the top of the browser window or on the tab of a browser.

     2. URL / Web Address: The name of the file is part of the URL. Where possible, use keywords in the file name.

     3. Headings: If the keywords are in a heading `<hn>` element then a search  engine will know that this page is all about that subject and give it greater weight than other text. 

     4. Text: Where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times. Do not, however, over-use these terms, because the text must be easy for a human to read.

     5. Link Text: Use keywords in the text that create links between pages (rather than using generic expressions such as "click here").

     6. Image Alt Text: Search engines rely on you providing accurate descriptions of images in the alt text. This will also help your images showup in the results of image-based searches.

     7. Page Descriptions: The description also lives inside the `<head>` element and is specified using a <meta> tag. It should be a sentence that describes the content of thepage. (These are not shown in the browser window but theymay be displayed in the results pages of search engines.)
    
    
  3. Off-Page Techniques: Getting other sites to link to you is just as important as on-page techniques. Search engines help determine how to rank your site by looking at the number of other sites that link to yours.
  
----

#### **How to Identify Keywords and Phrases:**

**Determining which keywords to use on your site can be one of the hardest tasks when you start to think about SEO. Here are six steps that will help you identify the right keywords and phrases for your site.**

  1. Brainstorm: List down the words that someone might type into  Google to find your site. Be sure to include the various topics, products or services your site is
about.

  2. Organize: Group the keywords into separate lists for the different sections or categories of your website.

  3. Research: There are several tools that let you enter your keywords and then they will suggest additional keywords you might like to consider, such as: 
     
     1. adwords.google.co.uk/select/KeywordToolExternal 
      
     2. www.wordtracker.com
     
     3. www.keyworddiscovery.com
  
  4. Compare: It is very unlikely that your site will appear at the top of  the search results for everykeyword. This is especially true  for topics where there is a lot of competition. The more sites out there that have already been  optimized for a given keyword, the harder it will be for you to  rise up the search results when people search on that term.
  
  5. Refine: Now you need to pick which keywords you will focus on. These should always be the ones that are most relevant to each section of your site.
  
  6. Map: Now that you have a refined list of keywords, you know which have the most competition, and which ones are most relevant, it is time to start picking which keywords you will use for each page.

----

#### **Analytics: Learning about your Visitors:** 

**soon as people start coming to your site, you can start analyzing how they found it, what they were looking at and at what point they are leaving. One of the best tools for doing this is a free service offered by Google called Google Analytics.**

  1. Signing Up: The Google Analytics service relies on you signing up for an account at: www.google.com/analytics The site will give you a piece of tracking code which you need to put on every page of your site.
  
  2. How it Works: Every time someone loads a page of your site, the tracking code sends data to the Google servers where it is stored. Google then provides a webbased interface that allows you to see how visitors use your site.
   
  3. The Tracking Code: A tracking code is provided by Google Analytics for each website you are tracking. It should appear just before the closing `</head>` tag. The code does not alter the appearance of your web pages.

      
---

> ## 3. History of Flash [Referance](https://en.wikipedia.org/wiki/Adobe_Flash#:~:text=The%20precursor%20to%20Flash%20was,computers%20running%20the%20PenPoint%20OS.)

[Flash Playes Logo](https://specials-images.forbesimg.com/imageserve/5f9c6af10985d5a5957cc4d5/960x0.jpg?fit=scale)

In the early 2000s, Flash was widely installed on desktop computers, and was often used to display interactive web pages and online games, and to play video and audio content. In 2005, YouTube was founded by former PayPal employees, and it used Adobe Flash Player as a means to display compressed video content on the web.

Between 2000 and 2010, numerous businesses used Flash-based websites to launch new products, or to create interactive company portals.Notable users include Nike, Hewlett-Packard (more commonly known as HP), Nokia, General Electric, World Wildlife Fund, HBO, Cartoon Network, Disney, and Motorola.After Adobe introduced hardware-accelerated 3D for Flash (Stage3D), Flash websites saw a growth of 3D content for product demonstrations and virtual tours.

In 2007, YouTube offered videos in HTML5 format to support the iPhone and iPad, which did not support Flash Player. After a controversy with Apple, Adobe stopped developing Flash Player for Mobile, focusing its efforts on Adobe AIR applications and HTML5 animation. In 2015, Google introduced Google Swiffy to convert Flash animation to HTML5, a tool Google would use to automatically convert Flash web ads for mobile devices. In 2016, Google discontinued Swiffy and its support.In 2015, YouTube switched to HTML5 technology on all devices; however, it would preserve the Flash-based video player for older web browsers


![Death of the crap](https://infosolblog.com/wp-content/uploads/2019/10/flashisdead-660x330.jpg)

---

Github Live: [view](https://anassawalha95.github.io/reading-notes-2/Class%2011)

Github Live: [view](https://github.com/anassawalha95/reading-notes-2/blob/main/Class%2011.md)
