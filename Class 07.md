> # Class 07 *Jan 11 2021:*

> ## Topics

   1. Domain Modeling [Referance](https://github.com/codefellows/domain_modeling#domain-modeling)
    
   2. Tables
    
   3. Functions, Methods, and Objects
    
   
   

---

> ## 1. Domain Modeling

#### **What is Domain Modeling?**

* **Domain model:** is a structured visual representation of interconnected concepts or real-world objects that incorporates vocabulary, key concepts, behavior, and relationships of all of its entities.

**A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.**

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

#### **Creating an Object Consructor Notation**

**The `new` Keyword and the object `constructor` create a blank object.**

![new and constructor](https://image.slidesharecdn.com/introductiontooojs-140127004826-phpapp01/95/introduction-to-object-oriented-javascript-6-638.jpg?cb=1390783865)


#### **Updating an Object**

* **To update the value of properties, use dot notation or square brackets. They work on objects created using literal or constructor notation. To delete a property use the delete keyword**




