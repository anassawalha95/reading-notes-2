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

    1. rgb values: These express colors in terms of how much red, green and blue are used to make it up. For 
    
    example:   `rgb(100,100,90)`
    
    ![RGB](https://i.pinimg.com/originals/43/39/57/4339577a1557730e777f490a2b71b8da.png)
    
    
    
    2. hex codes: These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign.
    
    example:   `#ee3e80`
    
    ![hex](https://i.pinimg.com/originals/e5/fa/00/e5fa0067c1273cc980ea4cfdc20d7a75.png)
    
    
    
    3. color names: There are 147 predefined color names that are recognized by browsers.
    
    example: `DarkCyan`
    
    ![color names](https://i.pinimg.com/originals/3b/35/3d/3b353d124b5b71e66011f6cd40003e7b.png)

    
    4. HSL color:  Stands for hue, saturation, and Lightness:
    
     1. hue: Hue is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be  shown as a slider with values from 0 to 360. 
     
     2. saturation: Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray. lightness       Lightness is the amount of white (lightness) or black (darkness) in a color. 

     3. Lightness is represented as a percentage.  0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as  luminosity.

    
     example: `hsl(180, 50%, 50%,0.9)`
    
    ![HSL](https://www.pngkey.com/png/detail/226-2265055_hsl-color-wheel-color-wheel-hue-saturation-value.png)

---


* **Color Contrast**

**Color Contrast:** is the difference in light between font (or anything in the foreground) and its background. To use color contrast you can apply:

   1. CSS `opacity` property: allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15%  opacity).
   
   example:  `opacity:0.3` 
   
   ![opacity](https://www.cssnewbie.com/wp-content/uploads/2017/07/box-opacity.jpg)
   
   2. rgba: which its the same as RGB where the letter "a" is for the opacity and stands for alpha .
   
   example:  `rgb(100,100,90,0.7)`
   
   ![rgba](https://codebridgeplus.com/wp-content/uploads/css3-colors-2-2.png)
   
   
   3. hsla: same as hsl where the letter "a" is for the opacity and stands for alpha.
   
   example: `hsl(180, 50%, 50%,0.9)`
   
   ![hsla](https://www.codeplannet.com/uploads/CodePlannet-File-33a6f8e9eb40cbbde223630fc548776f.PNG)
   
---

> ## 3. Text
