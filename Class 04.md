> # Class 04  *Jan 06 2021:* 

> ## Topics

__1. Links__
 
__2. Layout__

__3. Functions, Methods, and Objects__

__4. Pair Programming__

---

> ## 1. Links

![link](https://www.webdevelopersnotes.com/wp-content/uploads/html-links-target-attribute-of-anchor-tag.png)

* **Link:** are created using the `<a>` element. Users can click on anything between the opening `<a>` tag and the closing `</a>` tag. You specify which page you want to link to using the href attribute. 

* **Link Attribuites**
  
| Attribute | value                                       | Details                                                                     |
|-----------|---------------------------------------------|-----------------------------------------------------------------------------|
| href      | url                                         | Specifies the linked document, resource, or location.                       |
| title     | text                                        | Defines the title of a link, which appears to the user as a tooltip.        |
| target    |` _blank, _parent, _self, _top, _frame name` | Specifies the context in which the linked resource will open.               |
| download  |                                             | Directs the browser to download the linked resource rather than opening it. |
| hreflang  |                                             | Specifies the language of the linked resource.                              |


* **Relative Link Type:** Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.

![relative link type](https://thelinuxos.com/wp-content/uploads/2019/06/links.png)

* **Email Links:** we use `mailto: email-links.html` in HTML To create a link that starts up the user's email program and addresses an email to a specified email address, you use the <a> element. However, this time the value of the href attribute starts  with mailto: and is followed by the email address you want the email to be sent to.

![mailto](https://www.campaignmonitor.com/assets/uploads/2010/12/Should-I-Use-a-Mailto-or-Link-to-a-Contact-Form-in-My-Email-Newsletter.png)


* **Linking to a Specific Part of the Same Page:** At the top of a long page you might want to add a list of contents that links to the corresponding sections lower down. Or you might want to add a link from part way down the page back to the top of it to save users from having to scroll back to the top. 

Example: 

     <a href="#opening">Take me to the opening paragraph.</a>
     <p id="opening">Hyperlinks are utilized by a web browser to move from one page to another...</p>
     
     
* **Linking to a Specific Part of Another Page** to link to a specific part of a different page (whether on your own site or a different website) you  and the link the id

Example:
    
     <a href="youtube.com/#bottom">Take me to the end of the webpage.</a>
    

* **Directory Structure:** we have three main concepts:
  
  1. Structure:The diagram on the right shows the directory structure for a fictional entertainment listings website called ExampleArts.
  
  2. Homepages: The main homepage of a site written in HTML (and the homepages of each section in a child folder) is called index.html.
  
  3. Relationships: The relationship between files and folders on a website is described using the same terminology as a family tree.
  
  ![Directory Structure](https://stuyhsdesign.files.wordpress.com/2015/09/directory-structure1.png)



---

> ## 2. Layout
---

> ## 3. Functions, Methods, and Objects

---

>## 4. Pair Programming
