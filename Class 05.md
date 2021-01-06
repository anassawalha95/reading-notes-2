> # Class 04  *Jan 07 2021:*

> ## Topics

__1. Images__ 

__2. Color__ 

__3. Text__

---

> ## 1. Images

 * **Images are very engaging especially in well designed websites, consider the following tips for the best practices on adding and image:**

    1. relevant
    
    2. Convey information
    
    3. Convey the right mood
    
    4. Be instantly recognisable
    
    5. Fit the color palette

###  **Adding an Image:**

---

**use the `<img src="<url>" />` self closing tag to add an image to your website.**

Example:  

        <img src="images/quokka.jpg" alt="A family of quokka" title="The quokka is an Australian marsupial">
        
 
 ![img](https://www.miltonmarketing.com/wp-content/uploads/2018/03/mmhtmlimgtag424243image-tag-example.jpg)
 

 
 ###  **Image Attributes:**
 
 ----
 
| Attribute   | value                     | Details                                                       |
|-------------|---------------------------|---------------------------------------------------------------|
| src         | url                       | Specifies the path to the image                               |
| alt         | text                      | Specifies an alternate text for an image                      |
| crossorigin | anonymous use-credentials | Specifies the context in which the linked resource will open. |
| title       | text                      | Add image title                                               |
| width       | pixels                    | Specifies the width of an image                               |
| height      | pixels                    | Specifies the height of an image                              |


 ### **Image file Types:**
 
 ---

#### 1. **Image file formats:** are standardized means of organizing and storing digital images. An image file format may store data in an uncompressed format, a compressed format (which may be lossless or lossy), or a vector format

#### 2. **Type file formats:**

  ![Image file formats](https://www.graphicsmill.com/Aurigma/Images/GM7/image-formats.svg)
  
#### 3. **Tools to Edit & Save Images:** Below some of the best tools to edit images

  1. Skylum Luminar. 
  
  2. Adobe Photoshop. 
  
  3. DxO PhotoLab 4. 
  
  4. ON1 Photo RAW. 
  
  5. Corel PaintShop Pro. 
  
  6. ACDSee Photo Studio Ultimate. 
  
  7. GIMP.


---

> ## 2. Color

* **Color:** can make your webpages a live by blinding different cohenernt blended colors degrees. 

* **text color & Background Color:** Use `color` property to specify text color, in the mean while use `background-color` property to specify the background color of a web page. Also there are four different ways to set the color and its degree: 

    **1. **rgb values:** These express colors in terms of how much red, green and blue are used to make it up. For 
    
    example:   `rgb(100,100,90)`
    
    ![RGB](https://i.pinimg.com/originals/43/39/57/4339577a1557730e777f490a2b71b8da.png)
    
    
    
    **2. hex codes:** These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign.
    
    example:   `#ee3e80`
    
    ![hex](https://i.pinimg.com/originals/e5/fa/00/e5fa0067c1273cc980ea4cfdc20d7a75.png)
    
    
    
    **3. color names:** There are 147 predefined color names that are recognized by browsers.
    
    example: `DarkCyan`
    
    ![color names](https://i.pinimg.com/originals/3b/35/3d/3b353d124b5b71e66011f6cd40003e7b.png)

    
    **4. HSL color:**  Stands for hue, saturation, and Lightness:
    
     **1. hue:** Hue is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be  shown as a slider with values from 0 to 360. 
     
     **2. saturation:** Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray. lightness       Lightness is the amount of white (lightness) or black (darkness) in a color. 

     **3. Lightness:** is represented as a percentage.  0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as  luminosity.

    
     example: `hsl(180, 50%, 50%,0.9)`
    
    ![HSL](https://www.pngkey.com/png/detail/226-2265055_hsl-color-wheel-color-wheel-hue-saturation-value.png)

---


* **Color Contrast**

**Color Contrast:** is the difference in light between font (or anything in the foreground) and its background. To use color contrast you can apply:

   **1. CSS `opacity` property:** allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15%  opacity).
   
   example:  `opacity:0.3` 
   
   ![opacity](https://www.cssnewbie.com/wp-content/uploads/2017/07/box-opacity.jpg)
   
   **2. rgba:** which its the same as RGB where the letter "a" is for the opacity and stands for alpha .
   
   example:  `rgb(100,100,90,0.7)`
   
   ![rgba](https://codebridgeplus.com/wp-content/uploads/css3-colors-2-2.png)
   
   
   **3. hsla:** same as hsl where the letter "a" is for the opacity and stands for alpha.
   
   example: `hsl(180, 50%, 50%,0.9)`
   
   ![hsla](https://www.codeplannet.com/uploads/CodePlannet-File-33a6f8e9eb40cbbde223630fc548776f.PNG)
   
---

> ## 3. Text :

![Fonts](https://www.howtogeek.com/thumbcache/2/200/f6abb731c9c0a66c41036f15654b625e/wp-content/uploads/2015/01/BrowserFont-0.jpg)


* **Fonts:** font type is one of the main charstaristics in any webpage; in CSS we have different properties for fonts:

| Attribute    | value                                                                                                            | Details                                            |
|--------------|------------------------------------------------------------------------------------------------------------------|----------------------------------------------------|
| font-family  | serif, monospace, cursive, fantasy, caption, icon, menu, message-box, small-caption, status-bar, and "string"    | definies the font that is applied to the element.  |
| font-stretch | normal, ultra-condensed, extra-condensed, condensed, semi-condensed, semi-expanded, expanded, and extra-expanded | this property sets the font width                  |
| font-style   | normal, italic, oblique, inherit                                                                                 | makes the text appear italicised or oblique.       |
| font-variant | normal, small-caps                                                                                               | changes target text to small caps.                 |
| font-weight  | normal, bold, bolder, lighter, 100-900                                                                           | sets the weight or the thickness of the font.      |
| font-size    | xx-small, x-small, small, medium, large, x-large, xx-large, smaller, larger, percentage                          | sets the height of the font.                       |
| line-height  | normal, number (font-size multiplier), percentage                                                                | defines the amount of space above and below inline |


* **letter-spacing & word-spacing:** Kerning is the term typographers use for the space between each letter. Also the gap between words called words spacing.

**CSS Properties for letter-spacing & word-spacing:**

examples

   **1. letter-spacing**: `letter-spacing: 0.2em;`

   **2. word-spacing:**   `word-spacing: 1em;`
   
   
* **Alignment & vertical-align:**

**CSS Properties for alignment & vertical alignment:**

examples:

   **1. alignment**: `text-align: left;`

   **2. vertical-align:**   `vertical-align: text-top;`
   
* **Indenting Text:** allows you to indent the first line of text within an element. he amount you want the line indented by can be specified in a number of ways but is usually given in pixels or ems.

example:

   **text-indent:** `text-indent: 20px;`
  
* **Drop Shadow:** It is used to create a drop shadow, which is a dark version of the word just behind it and slightly offset. It can also be usedto create an embossed effect by adding a shadow that is slightly lighter than the text. 

example:

   **text-shadow:** `text-shadow: 1px 1px 0px #000000;`

* **First Letter or Line:** You can specify different values for the first letter or first line of text inside an element using  :first-letter and :first-line.

examples:

   **1. :first-letter** `p.intro:first-letter {font-size: 200%;}`
   
   **2. :first-line** `p.intro:first-line {font-weight: bold;}`


