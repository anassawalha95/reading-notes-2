
> # Class 01 *Jan 03 2021:*

> ## Topics
  
 * **101 & 102 Review:** 

   1. Web Pages Structure
    
   2. Extra Markup
    
   3. HTML5 Layout
    
   4. Process & Design
    
   5. Javascript The ABC of Programming
   
---

> ## 1. Web Pages Structure

![HTML Structure](https://www.development-tutorial.com/my_images/what_basic_structure_web_page/structure.png)


* HTML : stands for Hyper Text Markup Language.

* HTML pages are text documents.

* HTML uses tags (characters that sit inside angled brackets) to give the information they surround special meaning.

* Tags are often referred to as elements

* Tags usually come in pairs. The opening tag denotes the start of a piece of content; the closing tag denotes the end.

* Opening tags can carry attributes, which tell us more about the content of that element.

* Attributes require a name and a value.

* To learn HTML you need to know what tags are available for you to use, what they do, and where they can go.

**Example:**

![HTML Example](https://codescracker.com/html/images/html-document-structure-example.jpg)

---

> ## 2. Extra Markup

* **HTML Versions :** HTML 4 was introduced in 1997 with some exceptions of a few elements added in HTML5  Although HTML 4 had some presentational elements to control the appearance of pages, authors are not recommended to use them any more. (Examples include the <center> element for centering content on a page, <font> for controlling the appearance of text. although In 1998, a language called XML was published. Its purpose was to allow people to write new markup languages. Since HTML was the most widely used
markup language around, it was decided that HTML 4 should be reformulated to follow the rules of XML and it was renamed XHTML. In the mean while HTML 5 was introduced in 1997, In HTML5, web page authors do not need to close all tags, and new elements and attributes will be introduced. At the time of writing, the HTML5 specification had not been completed,but the major browser makers had started to implement many of the new features, and web page authors were rapidly adopting the new markup.

![HTML Versions](https://i.ytimg.com/vi/lcpEqOVHMXI/hqdefault.jpg)

* **DOCTYPE :** is declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included).

**Code Example:**

    For HTML 5
        <!DOCTYPE html>

    For HTML 4
        <!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">

* **Comments in HTML :**

    To add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:
        <!-- comment goes here -->


* **ID Attribute :** HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page

Example:

![ID Attribute](https://chaudharyacademy.com/wp-content/uploads/2020/11/frm00002-4.jpg)


* **Class Attribute :**

Example:

![Class Attribute](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRBU7HUaSwCvVPWgGSJ28jCejg8WLOR_IGrrg&usqp=CAU)


* **Information About Your Pages :** The <meta> element lives inside the <head> element and contains information about that web page. It is not visible to users but fulfills a  number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive. (If the page is time sensitive, it can be set to  expire.) The <meta> element is an empty element so it does not have a closing tag. It uses attributes to carry the information. 

![Meta Tag](https://www.webdevelopersnotes.com/wp-content/uploads/meta-tags-html-meta-tags-keyword-refresh-redirect.png)

* The value of the name attribute can be anything you want it to be. Some defined values for this attribute that are commonly used are:

  1. description: This contains a description of the page

  2. keywords: This contains a list of commaseparated words that a user might search on to find the page.
 
  3. robots: This indicates whether search engines should add this page to their search results or not.

  4. author: This defines the author of the web page.

  5. pragma: This prevents the browser from caching the page.

  6. expires: Because browsers often cache the content of a page, the expires option can be used to indicate when the page should expire (and no longer be cached).

Example: 

      <!DOCTYPE html>
      <html>
        <head>
          <title>Information About Your Pages</title>
          <meta name="description" content="An Essay on Installation Art" />
          <meta name="keywords" content="installation, art, opinion" />
          <meta name="robots" content="nofollow" />
          <meta http-equiv="author" content="Jon Duckett" />
          <meta http-equiv="pragma" content="no-cache" />
          <meta http-equiv="expires" content="Fri, 04 Apr 2014 23:59:59 GMT" />
        </head>
        <body>
        </body>
      </html>
---

> ## 3. HTML5 Layout 
 
* **HTML5 Layout:** provide a way to arrange web pages in well-mannered, well-structured, and in responsive form or we can say that HTML layout specifies a way in which the web pages can be arranged. Web-page layout works with arrangement of visual elements of an HTML document.

![HTML5 Layout](https://devdocs.magento.com/common/images/layouts_block_containers_defn21.png)

---

> ## 4. Process & Design

* There are very rich questionnaire before starting a new website to achieve a well-designed website or a business and here are some of it: 


 1. is the required website for an individual or a company?
 
 2. who's the targeted segment ? 
 
 3. is it global or local wide ?
 
 4. what is the preferable design?
 
 5. what type of the website is ?
 
* **Site Map:** The aim is to create a diagram of the pages that will be used to structure the site. 

![Site Map](https://i.pinimg.com/originals/1c/c5/f4/1cc5f4ec000969f11eedf4dbe0f8c9d8.png)

* **wireframe :** is a two-dimensional skeletal outline of a webpage or app. Wireframes provide a clear overview of the page structure, layout, information architecture, user low, functionality, and intended behaviors.

![wireframe](https://www.cleart.com/wp-content/uploads/2018/05/top-reasons-to-wireframe-your-web-or-mobile-app.jpg)

---

> ## 5. Javascript The ABC of Programming

* **What is Javascript:** JavaScript is a scripting or programming language that allows you to implement complex features on web pages — every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — you can bet that JavaScript is probably involved. It is the third layer of the layer cake of standard web technologies, two of which (HTML and CSS) we have covered in much more detail in other parts of the Learning Area.

![Javascript](https://mdn.mozillademos.org/files/13502/cake.png)



* **What is Flowchart:**  is a type of diagram that represents a workflow or process. A flowchart can also be defined as a diagrammatic representation of an algorithm, a step-by-step approach to solving a task.


![Flowchart](https://www.quality-assurance-solutions.com/images/flowchart-shapes-1.jpg)


* Example: 

![Flowchart Example](https://i.pinimg.com/originals/fc/b1/31/fcb13100330b8b483764c5ba75358a3a.png)


* **JS Example:** 

        <!DOCTYPE html>
        <html>
          <body>

            <h2>What Can JavaScript Do?</h2>

            <p id="demo">JavaScript can change HTML content.</p>

            <button type="button" onclick='document.getElementById("demo").innerHTML = "Hello JavaScript!"'>Click Me!</button>

          </body>
        </html>


Referance on Github: [Link](https://anassawalha95.github.io/reading-notes-2/Class%2001)
