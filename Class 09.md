> # Class 09 *Jan 13 2021:*

> ## Topics

   1. Forms
    
   2. Lists, Tables & Forms
    
   3. Events
    
   
   

---

> ## 1. Forms

* ** HTML form** is used to collect user input. The user input is most often sent to a server for processing

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
