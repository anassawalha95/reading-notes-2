> # Class 06 *Jan 10 2021:*

> ## Topics
 
   1. Object Literals
    
   2. Document Object Model
  
---


> ## 1. Object Literals

![js Object](https://javascript.info/article/object/object-user.svg)

### **What is the Object?**

**Objects:** group together a set of variables and functions to create a model
of a something you would recognize from the real world.

**Objects Properties:** is the variables inside the object body. If a function is part of an object, it is called a method.
Methods represent tasks that are associated with the object.

![js Object Properties](https://i.pinimg.com/originals/35/b2/42/35b2423677beefbb58f338e39eb853a7.jpg)

----

**Objects Methods:** If a function is part of an object, it is called a method.Methods represent tasks that are associated with the object.

![js Object Properties and methods](https://www.researchgate.net/profile/Henrique_Gaspar/publication/325361495/figure/fig1/AS:630136558858241@1527247671438/A-ship-as-a-JS-object-with-properties-eg-name-length-and-methods-eg-sail-idle.png)

----

### **Accessing an Object and Dot Notation:**

* **To accesse the properties of an object use object name then dot notation then add the variable name or the method name. Also you can use squre brackts**

![js Object access with dot notation and square brackts](https://dmitripavlutin.com/static/50a87420915de18f26da616865fe9825/05127/access-object-properties-2.png)


----

### **Creating objects:**

**You can create objects by defining a variable then opening a curly braces then adding a key value pairs.**

![Creating objects](https://d2tlksottdg9m1.cloudfront.net/uploads/2019/02/basic-JSON.jpg)

Example:

![Creating objects Example](https://image.slidesharecdn.com/javascript-110725163050-phpapp01/95/javascript-literacy-2-728.jpg?cb=1311612096)

---


> ## 2. Document Object Model


![Document Object Model](https://pbs.twimg.com/media/Dfgm4VPVAAEkcK5.jpg)


### **What is the Document Object Model?** 

* **The Document Object Model: (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.**

* **The DOM** specifies the way in which the browser should structure this model using a DOM tree.

* **Application Programming Interface (API):** Is another name for (Dom), User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other. The DOM states what your script can "ask the browser about the current page, and how to tell the browser to update what is being shown to the user.


![API](https://www.bbvaapimarket.com/wp-content/uploads/2016/06/bbva-open4u-que-hace-una-api-por-mi-negocio.png)

[API video Explanation](https://miro.medium.com/max/2560/1*v5HlKG-TIvm7BU5S34F1rw.png)

----

#### **Working With The DOM Tree**

* **Access The Elements:**

   1. Select an individual element node use
       
        1. getElementByld(): Uses the value of an element's id attribute
       
        2. querySelector(): Uses a CSS selector, and returns the first matching element.
       
   2. Select Multiple Elements (Node list):
   
       1. getElementsByClassName(): Selects all elements that have a specific value for their class attribute.
       
       2. getElementsByTagName(): Selects all elements that have the specified tag name .
       
       3. querySelectorAll(): Uses a CSS selector to select all matching elements.
   
   3. Traversing Between Element Nodes: 
 
       1. parentNode: Selects the parent of the current element node (which will return just one element). 
       
       2. previous Sibling / nextSibling: Selects the previous or next sibling from the DOM tree. 
       
       3. firstChild / lastChild: Select the first or last child of the current element.
   

* **Work With Elements:**

  1. Access/ Update Text Nodes
  
      1. nodeValue: This property lets you access or update contents of a text node.
      
      2. innerHTML: The text node does not include text inside any child elements. This property allows access to child elements and text content
      
      3. textContent: Same as innerHtml
      
      4. create Element(), createTextNode(), appendChild() / removeChild(): Several methods let you create new nodes, add nodes to a tree, and remove nodes from a tree. This is called DOM manipulation.
      
      5. className /id: Lets you get or update the value of the class and id attributes
      
      6. hasAttribute(), getAttribute(), setAttribute(), removeAttribute(): The first checks if an attribute exists. The second gets its value. The third updates the value. The fourth removes an attribute.
      

**Examples:**

**Creating an Element**

![Dom Creating and Element](https://codebrainer.azureedge.net/images/createElement_js_06.png)


**Updating an Element**

![Dom Updating and Element](https://blog.knoldus.com/wp-content/uploads/2018/11/html.png)



**Removing an Element**

![Dom Removing and Element](https://codebrainer.azureedge.net/images/createElement_js_09.png)


      
      
#### **Cross-Site Scripting (XSS) Attack:**

![XSS](https://i.ytimg.com/vi/oEFPFc36weY/maxresdefault.jpg)

* **XSS:** is a type of security vulnerability typically found in web applications. XSS attacks enable attackers to inject client-side scripts into web pages viewed by other users. A cross-site scripting vulnerability may be used by attackers to bypass access controls such as the same-origin policy.


**Some Simple code Example:**

   1. This first example stores cookie data in a variable, which could then be sent to a third-party server:

       `<script>var adr= 'http : //example.com/xss .php?cookie=' + escape(document . cookie);</script>`


   2. This code shows how a missing image can be used with an HTML attribute to trigger malicious code:

       `<img src="http://nofile" onerror="adr='http: //example.com/ xss .php?'+escape(document.cookie)";>`

----

#### Defending Against XSS:

![Defending Against XSS](https://www.articlediary.com/assets/cloud-hosting.png)


1. Validate Input Going to The Server:

   1. Only let visitors input the kind of characters they need to when supplying information. This is known as validation. Do not allow untrusted users to submit HTML markup or JavaScript.
   
   2. Double-check validation on the server before displaying user  ontent/storing it in a database.  This is important because users  could bypass validation in the browser by turning JavaScript off.  
   
   3. The database may safely contain markup and script from trusted sources (e.g., your  content management system). This is because it does not try to  process the code; it just stores it. 
   
2. Escape Data Coming From the Server & Database   

   1. As your data leaves the database, all potentially dangerous characters should be escape.
   
   2. Make sure that you are only inserting content generated by users into certain parts of the template files.
   
   3. Do not create DOM fragments containing HTML from untrusted sources. It should only be added as text once it has been escaped.
   
   
   
#### XSS Validation & Templates


1. Filter Or Validate Input: The most basic defense is to prevent users from entering characters into form fields that they do not need to use when providing that kind of information.


2. Limit Where User Content Goes: Malicious users will not just use <script> tags to try and create an XSS attack. As you saw on p228, malicious code can live in an event handler attribute without being wrapped in <script> tags. XSS can also be triggered by malicious code in CSS or URLs.


#### XSS Escaping & Controlling Markup

1. **Escaping User Content:** All data from untrusted sources should be escaped on the server before it is shown on the page. Most server-side languages offer helper functions that will strip-out or escape malicious code.

 Example:
      
 Escape these characters so that they are displayed as characters (not processed as code).

   1. `&` `&amp; &#x27; (not &apos;)`

   2. `<` `&lt; &quot;`

   3. `>` `&gt; I &#x2F;`

   4. `&#x60;`


2. **Adding User Content:** When you add untrusted content to an HTML page, once it has been escaped on the server, it should still be added to the page as text.
both offer tools for doing this:

-JAVASCRIPT: Never include data from untrusted sources in JavaScript. It involves escaping all ASCII characters with a value less than 256 that are not alphanumeric characters (and can be a security risk).

 Example:

   1. DO use: textContent or innerText

   2. DO NOT use: innerHTML 


-JQUERY

   1. DO use: `.text()`

   2. DO NOT use: `.html()`


3. **URLS:** If you have links containing user input (e.g., links to a user profile or search queries), use the JavaScript encodeURIComponent () method to encode the user input. It encodes the following characters:

 Example:

    `, I ? : @ & = + $ # `


**Notes:**
  
 * You can still use the innerHTML property and jQuery `.html()` method to add HTML to the DOM, but you must make sure that:
      
   1. You control all of the markup being generated (do not allow user content that could contain markup).
       
   2. The user's content is escaped and added as text using t he approaches noted above, rather than adding the user's content as HTML.
   
   

GitHub Live: [View](https://anassawalha95.github.io/reading-notes-2/Class%2006)

GitHub Repo: [View](https://github.com/anassawalha95/reading-notes-2)
