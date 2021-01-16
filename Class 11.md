> # Class 11 *Jan 17 2021:*

> ## Topics

  1. Images
  
  2. Practical Information
  
  3. History of Flash 

---

> ## 1. Images

![Images](https://webmeup.com/upload/blog/lead-image-105.png)

---

* **Controling Images Size in CSS:**

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

* **Aligning images:**

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

* **Centaring images:**

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

* **Background images**    

**You can insert an image in a backgound by :**

  1. `background-image`: allows you to place an image behind any HTML  element. This could be the entire page or just part of the page. By  default, a background image will repeat to fill the entire box.
  
 
**Example:**

    background-image: url("images/pattern.gif");}
  
---

* **Repeating Images:**    

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


---

* **Background Position:**

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

* **Images Rollover & Sprites**

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

* **CSS Gradients**

**CSS3 is going to introduce the ability to specify a gradient for the background of a box. The gradient is created using the background-image property and, at the time of writing, different browsers required a different syntax.**

**Examples:**

    background-image: -o-linear-gradient(#336666, #66cccc); 
    
---



> ## 2. Practical Information

---

> ## 3. History of Flash 



Github Live: [view](https://anassawalha95.github.io/reading-notes-2/Class%2011)

Github Live: [view](https://github.com/anassawalha95/reading-notes-2/blob/main/Class%2011.md)
