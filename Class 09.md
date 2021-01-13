> # Class 09 *Jan 13 2021:*

> ## Topics

   1. Forms
    
   2. Lists, Tables & Forms
    
   3. Events
    
   
   

---

> ## 1. Forms

* **HTML form** is used to collect user input. The user input is most often sent to a server for processing

![Forms](https://i2.wp.com/www.tutorialbrain.com/wp-content/uploads/2019/01/HTML-Form.jpg?fit=1920%2C1080&ssl=1)

#### **Form Structure**

    1. `<form>`: Form controls live inside a  `<form>` element. This element should always carry the action attribute and will usually have a method and id attribute too.

    2. action attribute: Its value is the URL for the page on the server that will receive the information in the form when it is submitted. 
    
    3. method attribute: can be sent using one of two methods: get or post.
    
    ![get or post](https://wtad640002.files.wordpress.com/2016/02/screenshot-481.png)
    

![Forms](https://cdn.educba.com/academy/wp-content/uploads/2019/06/html1.png)


#### **Text Input**    
      
      1. `type="text"`: When the type attribute has a value of text, it creates a singleline text input. 
      
      2. `name`: When users enter information into a form, the server needs to know which form control each piece of data was entered into. 
      
      3. `maxlength`: You can use the maxlength attribute to limit the number of characters a user may enter into the text field 
     
     
 #### **Password Input**        
 
      1. `type="password"`: When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out.
      
      2. size, maxlength It can also carry the size and  maxlength attributes like the the single-line text input.
      
      3. name: The name attribute indicates the name of the password input, which is sent to the server with the password the user enters.
      
#### **Textarea**  
      
      1. The `<textarea>` element  is used to create a mutli-line text input. Unlike other input elements this is not an empty element.
      
#### **Radio Button**       
      
      1. `type="radio"`: Radio buttons allow users to pick just one of a number of options.
      
      2. name: The name attribute is sent to the server with the value of the option the user selects.
      
      3. value: The value attribute indicates the value that is sent to the  server for the selected option.
      
      4. checked: The checked attribute can be used to indicate which value (if any) should be selected when the page loads.
      
#### **Radio Button**      

      1. `type="checkbox"`:  Checkboxes allow users to select (and unselect) one or more options in answer to a question.
      
      2. name:  The name attribute is sent to the server with the value of the option(s) the user selects.
      
      3. value: The value attribute indicates the value sent to the server if this checkbox is checked.
      
      4. checked: The checked attribute indicates that this box should be checked when the page loads. If used, its value should be checked.
      
#### **Drop Down List Box**   

      1. `<select>`: A drop down list box (also known as a select box) allows users to select one option from a drop down list.
   
      2. name: The name attribute indicates the name of the form control being sent to the server, along with the value the user selected.
      
      3. `<option>`: The <option> element is used to specify the options that the user can select from
      
      4. value: The <option> element uses the value attribute to indicate the value that is sent to the server along with the name of the control if this option is selected
      
#### **Multiple Select Box**   

      1. size: You can turn a drop down select box into a box that shows more than one option by adding the size attribute. Its value should be the number of options you want to show at once.
      
      2. multiple: You can allow users to select multiple options from this list by adding the multiple attribute with a value of multiple.

#### **File Input Box** 

      1. `<input>`: If you want to allow users to upload a file (for example an  image, video, mp3, or a PDF), you will need to use a file input box.
      
      2. `type="file"`: This type of input creates a box that looks like a text input followed by a browse button.
      
#### **Submit Button**      

      1. `type="submit"`: The submit button is used to send a form to the server.

      2. name: It can use a name attribute but it does not need to have one.
      
      3. value: The value attribute is used to control the text that appears on a button.
      
#### **Image Button**
      
      1. `type="image"`:  If you want to use an image for the submit button, you can give the type attribute a value ofimage. The src, width, height, and alt attributes work just like they do when used with the `<img>` element 

#### **Button & hidden Controls**     
      
      1. `<button>`: The `<button>` element was introduced to allow users more control over how their buttons  appear, and to allow other elements to appear inside the button.
      
      2. `<input>`: `type="hidden"`  This example also shows a hidden form control. These form  controls are not shown on the  page (although you can see them if you use the View Source option in the browser).
      
      
      
 
#### **Labelling Form Controls**     
      
      1. `<label>`: When introducing form controls,  the code was kept simple by  indicating the purpose of each one in text next to it.
      
      2. `for`: The for attribute states which form control the label belongs to. Note how the radio buttons use the id attribute.
      
      
#### **Grouping Form Elements**         
      
      1. `<fieldset>`: You can group related form controls together inside the  <fieldset> element. This is  particularly helpful for longer forms.
      
      2. `<legend>`: The <legend> element can  come directly after the opening  <fieldset> tag and contains a caption which helps identify the purpose of that group of form controls.
      

#### **Date Input**       

      1. `<input>`: Many forms need to gather  information such as dates, email addresses, and URLs.
      
      2. `type="date"`: If you are asking the user for a  date, you can use an `<input>` element and give the type attribute a value of date.
      
#### **Email & URL Input**         

      1. `type="email"`:  If you ask a user for an email address, you can use the email input. Browsers that support HTML5 validation will check that the user has provided information in the correct format of an email address. 
      
      2. `type="url"`: A URL input can be used when  you are asking a user for a web page address. 
      
#### **Search Input**

      1. `type="search"`:  If you want to create a single line text box for search queries
      
      2. `placeholder`: On any text input, you can also use an attribute called placeholder whose value is text that will be shown in the text box until the user clicks in that area.
      
     
     
     Example:
     
                <html>
                  <head>
                    <title>Forms</title>
                  </head>
                  <body>
                    <form action="http://www.example.com/review.php" method="get">
                      <fieldset>
                      <legend>
                      Your Details:
                      </legend>
                      <label>
                      Name:
                      <input type="text" name="name" size="30" maxlength="100">
                      </label>
                      <br />
                      <label>
                      Email:
                      <input type="email" name="email" size="30" maxlength="100">
                      </label>
                      <br />
                      </fieldset>
                      <br />
                      <fieldset>
                      <legend>
                      Your Review:
                      </legend>
                      <p>
                      <label for="hear-about">
                      How did you hear about us?
                      </label>
                      <select name="referrer" id="hear-about">
                      <option value="google">Google</option>
                      <option value="friend">Friend</option>
                      <option value="advert">Advert</option>
                      <option value="other">Other</option>
                      </select>
                      </p>
                      <p>
                      Example FORMS
                      Would you visit again?
                      <br />
                        <label>
                      <input type="radio" name="rating" value="yes" />
                      Yes
                      </label>
                      <label>
                      <input type="radio" name="rating" value="no" />
                      No
                      </label>
                        <label>
                       <input type="radio" name="rating" value="maybe" />
                      Maybe
                       </label>
                       </p>
                      <p>
                       <label for="comments">
                        Comments:
                        </label>
                        <br />
                         <textarea rows="4" cols="40" id="comments">
                        </textarea>
                        </p>
                       <label>
                       <input type="checkbox" name="subscribe" checked="checked" />
                       Sign me up for email updates
                        </label>
                       <br />
                        <input type="submit" value="Submit review" />
                      </fieldset>
                    </form>
                  </body>
                </html>
 
 ---
 
> ## 2. Lists, Tables & Forms
 

### 1. Lists

#### **Bullet Point Style**

* **The list-style-type property allows you to control the shape or style of a bullet point (also known as a marker).**
   
     1. Unordered Lists:
         
         1. none
         2. disc
         3. circle
         4. square
         
     2. Ordered Lists: For an ordered (numbered) list you can use the following values: 
         
         1. decimal: 1 2 3
         
         2. decimal-leading-zero: 01 02 03
         
         3. lower-alpha: a b c
         
         4. upper-alpha: A B C
         
         5. lower-roman: i. ii. iii.
         
         6. upper-roman: I II III
            
#### **Images for Bullets**
         
     * list-style-image: You can specify an image to act as a bullet point using the list-style-image property.     
     
#### **Images for Bullets**
   
     * list-style-position: Lists are indented into the page by default and the list-styleposition property indicates whether the marker should appear on the inside or the outside of the box containing the ain points.This property can take one of two values:
     
         1. outside The marker sits to the left of the block of text. (This is the default behaviour if this property is not used.)
         
         2. inside: The marker sits inside the box of text (which is indented).
     
#### **List Shorthand**

     * list-style: allows you to express the markers' style, image and position properties in any order.
---

### 2. Tables

#### **Table Properties**  

      1. width: to set the width of the table
      
      2. padding: to set the space between the border of each table cell and its content 
      
      3. text-transform: to convert the  content of the table headers to uppercase 
      
      4. letter-spacing, font-size:  to add additional styling to the content of the table headers  border-top, border-bottom to set borders above and below the table headers 
      
      5. text-align: to align the writing to the left of some table cells and to the right of the others

      6. background-color: to change the background color of the alternating table rows 
      
      7. :hover: to highlight a table row when a user's mouse goes over it
      
      8. Give cells padding If the text in a table cell either  touches a border (or another cell), it becomes much harder to read. Adding padding helps to improve readability. 

      9. Distinguish headings: Putting all table headings in bold (the default style for the `<th>` element) makes them easier to read. You can also make headings uppercase and then either add a background color or an underline to clearly distinguish them from content. 
      
      10. Shade alternate: rows Shading every other row canhelp users follow along the lines. Use a subtle distinction from the normal color of the rows to keep the table looking clean. 
      
      11. Align numerals: You can use the text-align property to align the content of any column that contains numbers to the right, so that large numbers are clearly distinguished from smaller ones.
      

#### **Border on Empty Cells**

      * empty-cells: use it to specify whether or not their  borders should be shown. It can take one of three values:
      
            1. show: This shows the borders of any empty cells.
            
            2. hide: This hides the borders of any empty cells.

            3. inherit: If you have one table nested  inside another, the inherit value instructs the table cells to obey the rules of the containing table.
            
#### **Gaps Between Cells**
           
      1. border-spacing: allows you to control the distance between adjacent cells. By default, browsers often leave  a small gap between each table cell, so if you want to increase or decrease this space then the border-spacing property allows you to control the gap. 
      
      2. collapse: Borders are collapsed into a single border where possible. (border-spacing will be ignored and cells pushed together, and empty-cells properties will be ignored.) 
      
      3. separate: Borders are detached from each other. (border-spacing and  empty-cells will be obeyed.) 
      
---

### 3. Styling Forms

####  **Styling Text Inputs**
      
      1. font-size: sets the size of the text entered by the user.
      
      2. color: sets the text color
      
      3. background-color: sets the background color of the input.
      
      4. border: adds a border around the edge of the input box.
      
      5. border-radius: can be used to create rounded corners.
      
      6. :focus pseudo-class: is used to change the background  color of the text input when it is being used
      
      7. background-image: adds a background image to the box. 
   
   
![cheatsheet](https://i.pinimg.com/originals/ae/ac/90/aeac9044ca81dcd5edc639e25db278c6.jpg)

Example:

      <!DOCTYPE html>
      <html>
      <head>
      <title>Lists, Tables and Forms</title>
      <style type="text/css">
      body {
      font-family: Arial, Verdana, sans-serif;
      font-size: 90%;
      color: #666;
      background-color: #f8f8f8;}
      li {
      list-style-image: url("images/icon-plus.png");
      line-height: 1.6em;}
      table {
      border-spacing: 0px;}
      th, td {
      padding: 5px 30px 5px 10px;
      border-spacing: 0px;
      font-size: 90%;
      margin: 0px;}
      th, td {
      text-align: left;
      background-color: #e0e9f0;
      border-top: 1px solid #f1f8fe;
      border-bottom: 1px solid #cbd2d8;
      border-right: 1px solid #cbd2d8;}
      tr.head th {
      color: #fff;
      background-color: #90b4d6;
      border-bottom: 2px solid #547ca0;
      border-right: 1px solid #749abe;
      border-top: 1px solid #90b4d6;
      text-align: center;
      text-shadow: -1px -1px 1px #666;
      letter-spacing: 0.15em;}
      td {
      text-shadow: 1px 1px 1px #fff;}
      tr.even td, tr.even th {
      background-color: #e8eff5;}
      tr.head th:first-child {
      -webkit-border-top-left-radius: 5px;
      -moz-border-radius-topleft: 5px;
      border-top-left-radius: 5px;}
      tr.head th:last-child {
      -webkit-border-top-right-radius: 5px;
      -moz-border-radius-topright: 5px;
      border-top-right-radius: 5px;}
      fieldset {
      width: 310px;
      margin-top: 20px;
      border: 1px solid #d6d6d6;
      background-color: #ffffff;
      line-height: 1.6em;}
      legend {
      font-style:italic;
      color:#666666;}
      input[type="text"] {
      width: 120px;
      border: 1px solid #d6d6d6;
      padding: 2px;
      outline: none;}
      input[type="text"]:focus,
      input[type="text"]:hover {
      background-color: #d0e2f0;
      border: 1px solid #999;}
      input[type="submit"] {
      border: 1px solid #006633;
      background-color: #009966;
      color: #FFFFFF;
      border-radius: 5px;
      padding: 5px;
      margin-top: 10px;}
      input[type="submit"]:hover {
      border: 1px solid #006633;
      background-color: #00CC33;
      color: #FFFFFF;
      cursor: pointer;}
      .title {
      float: left;
      width: 160px;
      clear: left;}
      .submit {
      width: 310px;
      text-align: right;}
      </style>
      </head>
      <body>
      <h1>Poetry Workshops</h1>
      <p>We will be conducting a number of poetry workshops
      and symposiums throughout the year.</p>
      <p>Please note that the following events are free to
      members:</p>
      <ul>
      <li>A Poetic Perspective</li>
      <li>Walt Whitman at War</li>
      <li>Found Poems and Outsider Poetry</li>
      </ul>
      <table>
      <tr class="head">
      <th></th>
      <th>New York</th>
      <th>Chicago</th>
      <th>San Francisco</th>
      </tr>
      <tr>
      <th>A Poetic Perspective</th>
      <td>Sat, 4 Feb 2012<br />11am - 2pm</td>
      <td>Sat, 3 Mar 2012<br />11am - 2pm</td>
      <td>Sat, 17 Mar 2012<br />11am - 2pm</td>
      </tr>
      <tr class="even">
      <th>Walt Whitman at War</th>
      <td>Sat, 7 Apr 2012<br />11am - 1pm</td>
      <td>Sat, 5 May 2012<br />11am - 1pm</td>
      <td>Sat, 19 May 2012<br />11am - 1pm</td>
      </tr>
      <tr>
      <th>Found Poems `&amp;` Outsider Poetry</th>
      <td>Sat, 9 Jun 2012<br />11am - 2pm</td>
      <td>Sat, 7 Jul 2012<br />11am - 2pm</td>
      <td>Sat, 21 Jul 2012<br />11am - 2pm</td>
      </tr>
      <tr class="even">
      <th>Natural Death: An Exploration</th>
      <td>Sat, 4 Aug 2012<br />11am - 4pm</td>
      <td>Sat, 8 Sep 2012<br />11am - 4pm</td>
      <td>Sat, 15 Sep 2012<br />11am - 4pm</td>
      </tr>
      </table>
      <form action="http://www.example.com/form.php" method="get">
      <fieldset>
      <legend>Register your interest</legend>
      <p><label class="title" for="name">Your name:</label>
      <input type="text" name="name" id="name"><br />
      <label class="title" for="email">Your email:</label>
      <input type="text" name="email" id="email"></p>
      <p><label for="location" class="title">Your closest center:</label>
      <select name="location" id="location">
      <option value="ny">New York</option>
      <option value="il">Chicago</option>
      <option value="ca">San Francisco</option>
      </select></p>
      <span class="title">Are you a member?</span>
      <label><input type="radio" name="member" value="yes" /> Yes</label>
      <label><input type="radio" name="member" value="no" /> No</label></p>
      </fieldset>
      <div class="submit"><input type="submit" value="Register" /></div>
      </form>
      </body>
      </html>
---


> ## 3. Events

#### **What is Evnets? **

* **When you browse the web, your browser registers different types of events. It's the browser's way of saying, "Hey, this  just happened." Your script can then respond to these events.**

#### **JavaScript Event**

 ![Event](https://i.pinimg.com/originals/79/93/f5/7993f58253f6dfd2d356347e6820ac32.jpg)     



#### **JavaScript Event Listeners**

* **Event listeners are a more recent approach to handling events. They can deal with more than one function at a time but they are not supported in older browsers.** 

![Event listeners ](https://cdn.tutsplus.com/active/uploads/legacy/flashtuts/074_EventListenersBasics/1.jpg)

  
Example:

![ Event listeners ex](https://miro.medium.com/max/2784/1*xPmfzRHrKitsqurnA8usOw.png)

#### **Event Flow:**

![Event flow](https://cdn.javascripttutorial.net/wp-content/uploads/2020/02/JavaScript-DOM-Level-2-Event.png)


Github Live: [View](https://anassawalha95.github.io/reading-notes-2/Class%2009)
Github Repo: [View](https://github.com/anassawalha95/reading-notes-2/blob/main/Class%2009.md)
