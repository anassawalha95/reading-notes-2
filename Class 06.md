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


![API](https://qatestlab.com/assets/Uploads/API-Application-Programming-Interface.)

[API video](https://miro.medium.com/max/2560/1*v5HlKG-TIvm7BU5S34F1rw.png)

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

**Creating an Element **

![Dom Creating and Element](https://codebrainer.azureedge.net/images/createElement_js_06.png)


**Updating an Element **

![Dom Updating and Element](https://blog.knoldus.com/wp-content/uploads/2018/11/html.png)



**Removing an Element **

![Dom Removing and Element](https://codebrainer.azureedge.net/images/createElement_js_09.png)


      
      
* **Cros**





