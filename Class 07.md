> # Class 07 *Jan 11 2021:*

> ## Topics

   1. Domain Modeling [Referance](https://github.com/codefellows/domain_modeling#domain-modeling)
    
   2. Tables
    
   3. Functions, Methods, and Objects
    
   
   

---

> ## 1. Domain Modeling

#### **What is Domain Modeling?**

* **Domain model:** is a structured visual representation of interconnected concepts or real-world objects that incorporates vocabulary, key concepts, behavior, and relationships of all of its entities.

* **A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.**

![Domain Modeling](https://sparxsystems.com/enterprise_architect_user_guide/14.0/images/domain-model-5600.png)

---

> ## 2. Tables

#### **What is Tables?**

* **Tables:** A table represents information in a grid format.

![Tables](https://mdn.mozillademos.org/files/14587/swimming-timetable.png)

----

#### **Table Structure**

* **Table Tags:**

   1. `<table>`: The `<table>` element is used to create a table. The contents of the table are written out row by row.
   
   2. `<th>`: The `<th>` element is used just like the `<td>` element but its purpose is to represent the heading for either a column or  a row.
   
   3. `<tr>`: You indicate the start of each row using the opening `<tr>` tag.
   
   4. `<td>`: Each cell of a table is represented using a `<td>` element. (The td stands for table data.)
   
   5. `<thead>`: The headings of the table should sit inside the `<thead>` element. 
   
   6. `<tbody>`: The body should sit inside the `<tbody>` element.

   7. `<tfoot>`: The footer belongs inside the `<tfoot>` element.


   **Example**
   
         <table>
         <thead>
            <tr>
               <th></th>
               <th scope="col">Home starter hosting</th>
               <th scope="col">Premium business hosting</th>
            </tr>
         </thead>
         <tbody>
            <tr>
               <th scope="row">Disk space</th>
                  <td>250mb</td>
                  <td>1gb</td>
               </tr>
               <tr>
                  <th scope="row">Bandwidth</th>
                  <td>5gb per month</td>
                  <td>50gb per month</td>
               </tr>
         </tbody>
         <tfoot>
            <tr>
               <td></td>
               <td colspan="2">Sign up now and save 10%!</td>
            </tr>
         </tfoot>
         </table>
   
   
---

> ## 3. Functions, Methods, and Objects

#### * **Creating an Object Consructor Notation**

* **The `new` Keyword and the object `constructor` create a blank object.**

![new and constructor](https://image.slidesharecdn.com/introductiontooojs-140127004826-phpapp01/95/introduction-to-object-oriented-javascript-6-638.jpg?cb=1390783865)


#### * **Updating an Object**

* **To update the value of properties, use dot notation or square brackets. They work on objects created using literal or constructor notation. To delete a property use the delete keyword**


![update & Delete object Properties](https://flaviocopes.com/how-to-remove-object-property-javascript/delete-object-property.png)

----


#### * **Creating Many Objects: Constructor Notation**

* **Object constructors can use a function as template for creating objects**

![Creating Many Objects](https://miro.medium.com/max/1964/1*FV5pGUFrVhshmxQI9WdsuA.png)

----


#### * **`this` Its A Keyword**

* **`this` Keyword:** `this` is commonly used inside functions and objects where the function is declared alters what `this` mean. It always refers to one object, usually the object in which the function operates 

![this keyword](https://www.tutorialsteacher.com/Content/images/oo-js/this-global.png)


----


#### * **Arrays Are Objects**

* **Arrays:** are actually a special type of object. They hold a related set of key/value pairs (like all objects), but the key for each value is its index number.

**Object**

| Property | Value  |
|----------|--------|
| Mercedes | $20000 |
| BMW      | $35000 |
| kie      | $100   |

**Array**

| Index | Value  |
|-------|--------|
|   0   | $20000 |
|   1   | $35000 |
|   2   |  $100  |

----

#### * **Arrays of Objects & Objects in Arrays**

* **You can combine arrays and objects to create complex data structures: Arrays can store a series of objects (and remember their order). Objects can also hold arrays (as values of their properties)**


**Arrays in an Object:**

| Index    | Value                           |
|----------|---------------------------------|
| Mercedes | `Prices[$20000,$32500,$15350]`  |
|    BMW   | `Prices[$140000,$30500,$10000]` |
|    kie   |     `Prices[$100,$50,$0.25]`    |


**Objects in an Array:**


| Index | Value                     |
|-------|---------------------------|
|   0   | `{$20000,$32500,$15350}`  |
|   1   | `{$140000,$30500,$10000}` |
|   2   |     `{$100,$50,$0.25}`    |

----

#### * **Built in Objects**

* **Browsers come with a set of built-in objects that represent things like the browser window and the current web page shown in that window. These built-in objects act like a toolkit for creating interactive web pages.**

* **There are Three Groups of Built in Objects**

1. **Brower Object Model (BOM):** Creates a model of the browser tab or window 


![Brower Object Model](https://image.slidesharecdn.com/013browserobjectmodel-190503092234/95/javascript-chapter-13-browser-object-modelbom-5-638.jpg?cb=1556875428)


2. **Document Object Model (DOM):** Create model of the current web page.

![Document Object Model](https://www.pierre-giraud.com/wp-content/uploads/2019/11/javascript-representation-dom.jpg)


3. **Global Javascript Objects:** It doesn't form a single model. They are a group of individual objects that relate to different parts of the JavaScript language


![Global Javascript Objects](https://res.cloudinary.com/practicaldev/image/fetch/s--jRLu_Z5j--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/q6pyi9z2qpt9iai9foqx.png)


![Recap DOM,BOM, and Global Javascript Objects ](https://javascript.info/article/browser-environment/windowObjects.svg)



GitHub live: [View](https://anassawalha95.github.io/reading-notes-2/Class%2007)

GitHub Repo: [View](https://github.com/anassawalha95/reading-notes-2/)

