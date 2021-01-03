> # Class 03 *Jan , 5, 2021:*

> ## Topics

__1. Lists__ 

__2. Boxes__ 

__3. Basic JavaScript Instructions__

__4. Decisions & Loops "switch statements"__

---

> ## 1. Lists

- In Html there are three types of lists:

  * Ordered Lists: where all items in the list are numbered
  
  Example: 
  
    ` <ol>`
    
    ` <li> First Item </li>` 
       
    ` <li> Second Item </li>` 
       
    ` <li> Third Item </li>` 
        
    ` </ol>` 
    
   
       Result:

             1. First Item
             2. Second Item
             3. Third Item

    
  * Unordered Lists: whrere items begins with a bullet point
  
   Example: 
    
    ` <ul>`
    
    ` <li> First Item </li>`
    
    ` <li> Second Item </li>`
     
    ` <li> Third Item </li>`
     
    ` </ul> `
   
   
      
        Result:
    
              * First Item

              * Second Item

              * Third Item
      
  
  * Definition Lists: are made up of a set of terms along with the definitions for each of those terms.
   Example:
   
    ` <dl>`
      
    ` <dt> 1 Item </dt>`
       
    ` <dd> First Item </dd>`
        
    ` <dt> 2 Items </dt>`
        
    ` <dd> Second Item </dd>`
        
    ` <dd> Third Item </dd>`
        
    ` </dl>`

        Result:

         1 Item 

             First Item

         2 Items

             Second Item 

             Third Item

    
---

> ## 2. Boxes

* Box: is sized just big enough to hold its contents. 

* To set dimensions for a box you can use the height and width properties:

 Example:
 
       <div>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
          Corporis laudantium quidem earum hic quos dolore,
          cupiditate iure facere pariatur vitae iste quas velit aliquam. Voluptate,
          reprehenderit! Eveniet laborum saepe labore!</p>
       </div>
       
       
       div.box {
       height: 300px;
       width: 300px;
       background-color: #bbbbaa;}
       p {
       height: 75%;
       width: 75%;
       background-color: #0088dd;}
       
* To Limit dimensions for a box you can use the min-height,max-hight, min-width, max-width properties:
     
 Example: 
 
       div.box {
       min-height: 200px;
       max-width: 300px;
       background-color: #bbbbaa;}
       p {
       max-height: 75%;
       min-width: 75%;
       background-color: #0088dd;}
       
* overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:  

 1. hidden: This property simply hides any extra content that does not fit in the box.
 
 2. scroll: This property adds a scrollbar to the box so that users can scroll to see the missing content.
 
 Example: 
   
      p.one {
      overflow: hidden;}
      p.two {
      overflow: scroll;}
      
      
 * Margin, Border & Padding:
 
  ![Margin, Border & Padding](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQThj10hsc4sNgrelzln9XWgf_63cnYwGcVgA&usqp=CAU)
 
  1. Margin: The margin property controls the gap between boxes.
  
         margin-left:5px;
         margin-right:5px;
         margin-top:5px;
         margin-bottom:5px;
         
         or
          
         margin:5px 5px 5px 5px;
     
   Note:  for centering element set margin left and right to auto   
   
 
  2. Border property allows you to specify the width, style and color of a border
   
   Example: 
     
         border-style: dotted ;
         border-size: 3px ;
         border-color:#0088dd;
         
         or
         
         border: solid 5px #000000;
         
         
         
  3. padding: The padding property allows you to specify how much space should appear between the content of an element and its border.
  
   Example: 
         
         padding-left:5px;
         padding-right:5px;
         padding-top:5px;
         padding-bottom:5px;
         
         or
         
         padding:5px 5px 5px 5px;
         
         
 * Display: The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page.
 
   display values are: 
     
     1. inline: This causes a block-level element to act like an inline element.
     
     2. block: This causes an inline element to act like a block-level element.
     
     3. inline-block: This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.
     
     4. none: This hides an element from the page.
     
  
  Example:
  
       display:inline;
       display:block;
       display:inline-block;
       display:none;
       
       
* Box Shadow: The box-shadow property allows you to add a drop shadow around a box.

  ![Box Shadow](https://s3-us-west-2.amazonaws.com/s.cdpn.io/66763/box-shadow-syntax.png)
  
   Example:
       
          box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
          
          
* Rounded Corners: introduce the ability to create rounded corners on any box

 ![Rounded Corners]( https://www.the-art-of-web.com/images/border-radius.gif)
  
 Example:
       
          border-radius: 25px;
 
 
 
#### Copy and Paste This Example to your index.html :   

          <!DOCTYPE html>
           <html>
           <head>
             <title>Boxes</title>
             <style type="text/css">
                body {
                font-size: 80%;
                font-family: "Courier New", Courier, monospace;
                letter-spacing: 0.15em;
                background-color: #efefef;}
                #page {
                max-width: 940px;
                min-width: 720px;
                margin: 10px auto 10px auto;
                padding: 20px;
                border: 4px double #000;
                background-color: #ffffff;}
                #logo {
                width: 150px;
                margin: 10px auto 25px auto;}
                ul {
                width: 570px;
                padding: 15px;
                margin: 0px auto 0px auto;
                border-top: 2px solid #000;
                border-bottom: 1px solid #000;
                text-align: center;}
                li {
                display: inline;
                margin: 0px 3px;}
                p {
                text-align: center;
                width: 600px;
                margin: 20px auto 20px auto;
                font-weight: normal;}
                BOXES 326
                Example
                BOXES
                a {
                color: #000000;
                text-transform: uppercase;
                text-decoration: none;
                padding: 6px 18px 5px 18px;}
                a:hover, a.on {
                color: #cc3333;
                background-color: #ffffff;}
             </style>
           </head>
           <body>
            <div id="page">
            <div id="logo">
            <img src="images/logo.gif" alt="The Analog Specialists" />
            </div>
            <ul id="navigation">
              <li><a href="#" class="on">Home</a></li>
              <li><a href="#">For Sale</a></li>
              <li><a href="#">Repairs</a></li>
              <li><a href="#">About</a></li>
              <li><a href="#">Contact</a></li>
            </ul>
            <p>
            <img src="images/keys.jpg" alt="Fender Rhodes, Hohner Clavinet,
            and Wurlitzer EP200" />
            </p>
            <p>
            We specialise in the sales and repair of classic keyboards, in particular
            the Fender Rhodes, Wurlitzer EP200, and Hohner Clavinet.
            </p>
            </div>
           </body>
          </html>
 
---

> ## 3. Basic JavaScript Instructions:
 
* Arrays: An array is a special type of variable. It doesn't just store one value; it stores a list of values.

 ![Arrays](https://media.geeksforgeeks.org/wp-content/uploads/C-Arrays.jpg)
    
    1. consider using an array whenever you are working with a list or a set of values that are related to each other.
    2. Arrays are especially helpful when you do not know how many items a list will contain.
    
 * Creating an Array: 
     
    Example: 
         
         var colors;
         colors ['white', 'black', ' custom '];
         
         or 
         
         var colors = new Array('white ' , 'black', 'custom ' );
         
 * Values in Arrays: each item in an array is automatically given a number called an index. This can be used to access specific items in the array.
   
        var colors;
        colors= ['white' ,'black ' ,' custom'];
        
        INDEX   VALUE
          0     'white'
          1      'black'
          2     'custom'
        
* Accessing Items in an Array: To retrieve the third item on the list of the above example, the array name is specified along with the index number in square brackets.

        var itemThree;
        itemThree = colors [2] ;
        
* Number of Items In an Array: Each array has a property called length, which holds the number of items in the array

        var numColors ;  
        numColors =col ors. length;
        
---

> ## 4. Decisions & Loops "Switch Statements":
 
* The Switch Statements:  A switch statement starts with a variable called the switch value.Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

For Example: 

      switch (level) {
          case 'One ':
          title= 'Level 1 ' ;
          break;
          case 'Two':
          title = ' Level 2 ' ;
          break;
          case ' Three' :
          title = 'Level 3' ;
          break ;
          default :
          title= 'Test';
          break;
        }


IF....Else  VS  SWITCH

| IF ... ELSE                                                                                                                   | SWITCH                                                                                                                                                                      |
|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| There is no need to provide an else   option. (You can just use an if option.  (You can just use an if statement.)            | You have a default option that is run if none of the cases match.                                                                                                           |
| With a series of if statements, they are all checked even if a match has been found (so it performs more slowly than switch). | If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing better performance than multiple i f statements). |




