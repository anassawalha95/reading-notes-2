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

![Layout](https://media.emailonacid.com/wp-content/uploads/2019/05/EOA_BackgroundColorsImages2019_Blog.gif)


* **Building Blocks:** CSS treats each HTML element as if it is in its own box. This box will either be:
  
    1. block-level box: start on a new line and act as the main building blocks of any layout.
    
    2. inline box: flow between surrounding text.
   
   ![Building Blocks](https://media.gcflearnfree.org/content/5e82363212da9215e057b928_03_30_2020/block_vs_inline_diagram.png)


* **Containing Elements:** If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. 

* **Controlling the Position of Elements**
---

* **CSS has the following positioning schemes that allow you to control the layout of a page:**
   
   1. Normal flow: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one, this is the default behavior.
   
   2. Relative Positioning: This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.
   
   3. Absolute positioning: This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up).  Absolutely positioned elements move as users scroll up and down the page.  
   4. Fixed Positioning: This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down the page.
   
   5. Floating Elements Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.
   
 ![Positioninig](https://www.csssolid.com/images/csspositions/css-position-all.png)  
 
 
 * **z-index:** property specifies the stack order of an element. An element with greater stack order is always in front of an element with a lower stack order. Note: z-index only works on positioned elements (position: absolute, position: relative, position: fixed, or position: sticky). Default value: auto. 
 
  ![z-index](https://spyrestudios.com/wp-content/uploads/css-z-index-c87ef0.png)  
  
 * **float property** allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.
  
 
  ![float](https://www.1keydata.com/css-tutorial/example-float-right-float-left.jpg)
  
  
  * **clear property** allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values: 
      
      1. left 
      
      2. right
      
      3. both
      
      
 ![clear](https://qph.fs.quoracdn.net/main-qimg-6a0fefa98cdada11845be463db7000aa) 
 
 * **Screen Sizes:** Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

* **Screen Resolution** Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens

* **Page Sizes** Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).  

![responsive](https://s3.amazonaws.com/blog.invisionapp.com/uploads/2018/02/slack-responsive-web-design.png)
 
 Example: Try Copy and Paste to your index.html or view it [Click Me To view it](https://codepen.io/anas-sawalhah/full/oNjJyGY)
 
                 <!doctype html>
          <html>
          <head>
          <meta charset="utf-8">
          <title>Landing Page</title>
          <script src="https://use.fontawesome.com/35c8fc8d0f.js"></script> <!-- fontawesome--> 
          <script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.13.0/js/all.min.js"></script>
          <style>
          * {
              margin: 0px;
              padding: 0px;
              box-sizing: border-box;
          }
          body {
              padding: 10px;
              display: block;
              background-color: #eee;
          }
          #header {
              position: fixed;
              left: 0px;
              top: 0px;
              display: flex;
              align-items: center;
              justify-content: space-around;
              background-color: #ddd;
              width: 100%;
              padding: 17px 20px;
              z-index: 1;
          }

          @media (max-width:600px) {
          #header {
              flex-wrap: wrap;
          }
          }
          #logo {
              display: flex;
              justify-content: flex-start;
              align-items: center;
              width: 100%;
              height: 100%;
          }
          #header-img {
              width: 100%;
              height: 100%;
              max-width: 280px;
          }
          #nav-bar>ul {
              display: flex;
              list-style: none;
              flex-direction: row;
              width: 51vw;
              justify-content: space-around;
              align-items: center;
              text-align: center;
          }
          #nav-bar a {
              color: black;
              text-decoration: none;
          }

          @media (max-width:600px) {
          #nav-bar>ul {
              flex-direction: column;
              margin-top: 10px;
          }
          #nav-bar>ul>li {
              flex-direction: column;
              margin-top: 10px;
          }
          }
          .container {
              display: block;
              margin: 0 auto;
              max-width: 1000px;
          }
          section {
              display: block;
              margin: 80px auto;
          }
          #hero {
              display: flex;
              flex-direction: column;
              justify-content: center;
              align-items: center;
          }

          @media (max-width:600px) {
          #hero {
              margin-top: 36vw;
          }
          }
          #hero input["email"] {
          margin-top: 30px;
          width: 100%;
          max-width: 250px;
          }
          #form {
              width: 100%;
              max-width: 300px;
          }
          #hero input[type="email"] {
              display: block;
              width: 100%;
              max-width: 231px;
              margin: 15px auto;
              padding: 10px;
              border-radius: 5px;
              border-width: 3px;
              border-color: white;
              border-style: solid;
              outline: none;
          }
          .btn {
              display: block;
              padding: 15px;
              border-color: #ffce1a;
              border-radius: 5px;
              background-color: #ffce1a;
              border-style: solid;
              margin: 0 auto;
              font-weight: bold;
              box-shadow: 1px 8px 2.2px rgba(243, 7, 7, 0.13), 0 6.7px 5.3px rgba(255, 0, 0, 0.23), 0 12.5px 10px rgba(0, 0, 0, 0.06), 0 22.3px 17.9px rgba(255, 30, 30, 0.072), 0 41.8px 33.4px rgba(255, 14, 14, 0.086), 0 100px 80px rgba(0, 0, 0, 0.12);
              animation-name: clk;
              animation-duration: 1s;
              outline: none;
          }
          .btn:hover {
              animation-name: hov1;
              animation-duration: 2s;
              animation-fill-mode: forwards;
              cursor: pointer;
          }
          #hero input[type="email"]:focus {
              animation-name: hov2;
              animation-duration: 500ms;
              animation-fill-mode: forwards;
              animation-timing-function: ease;
          }
          @keyframes clk {
          from {
          box-shadow:  1px 8px 2.2px rgba(243, 7, 7, 0.13), 0 6.7px 5.3px rgba(255, 0, 0, 0.23), 0 12.5px 10px rgba(0, 0, 0, 0.06), 0 22.3px 17.9px rgba(255, 30, 30, 0.072), 0 41.8px 33.4px rgba(255, 14, 14, 0.086), 0 100px 80px rgba(0, 0, 0, 0.12);
          }
          to {
          box-shadow:  1px 8px 2.2px rgba(243, 7, 7, 0.13), 0 6.7px 5.3px rgba(255, 0, 0, 0.23), 0 12.5px 10px rgba(0, 0, 0, 0.06), 0 22.3px 17.9px rgba(255, 30, 30, 0.072), 0 41.8px 33.4px rgba(255, 14, 14, 0.086), 0 100px 80px rgba(0, 0, 0, 0.12);
          }
          }
          @keyframes hov1 {
          from {
          border-color: #ffce1a;
          }
          to {
          border-color:#24C5D3;
          }
          }
          @keyframes hov2 {
          from 0% {
          outline: none;
          }
          100% {
          outline: solid;
          outline-width: 3px;
          outline-color:#24C5D3;
          }
          }
          .main_feature {
              display: flex;
              margin: 43px auto;
          }
          .icon {
              display: flex;
              justify-content: center;
              color: orange;
              width: 8vw;
              padding: 0px 0px 0px 15px;
              align-items: center;
              height: 73px;
          }
          .desc {
              padding: 0px 0px 0px 25px;
          }
          #video {
              display: block;
              margin: 0 auto;
          }
          #Pricing {
              display: flex;
              flex-direction: row;
              justify-content: flex-start;
          }
          .price {
              display: flex;
              flex-direction: column;
              justify-content: space-around;
              flex-wrap:wrap;
              align-items: center;
              width: calc(100% / 3);
              background-color: #E3E3E3;
              border-color: black;
              border-width: 2px;
              border-style: solid;

              margin-left: 10px;
              border-radius: 5px;
              text-align: center;
              list-style: none;
          }

           @media (max-width:650px){
            #Pricing{

             flex-wrap:wrap;
              justify-content: center;
            }
            .price{
             width: 100%;
             max-width: 250px;
             margin-bottom: 10px;


            }

           }
          .card-head {
              display: block;
              background-color: #cecece;
              width: 100%;
              padding: 16px;
          }
          .card-content>h2 {
              padding: 20px;
          }
          .card-content>ul {
              list-style: none;
              padding: 0px 0 20px 0
          }
          .card-content>ul>li {
              padding: 0px 0 20px 0
          }
          .card-content div {
              height: 74px;
              width: 100%;
          }
          .card-content .btn {
              padding: 7px;
              border-radius: 2px;
           font-style: italic;
           font-weight: bold;
          }
           #footer{
            width: 100%;
              padding: 15px;
              background-color: #cecece;
              height: 100%;
              display: flex;
              justify-content: flex-end;

           }


           #footer-content{
                display: flex;
              flex-direction: column;

           }
           #footer-link{
           display: flex;
              justify-content: space-around;

           }
           #footer-link>a{
           text-decoration: none;
            color: black;

           }
           #copy-right{
            color: #353333;
            font-size: 15px;
            font-style: italic;
            padding: 5px;

           }
          </style>
          </head>

          <body>
          <header id="header">
            <div id="logo"> <img src="https://s3.amazonaws.com/freecodecamp/original_trombones.png" alt="original trombones logo" id="header-img"> </div>
            <nav id="nav-bar">
              <ul>
                <li><a href="#features">Features</a></li>
                <li><a href="#How-It-Works">How It Works</a></li>
                <li><a href="#Pricing">Pricing</a></li>
              </ul>
            </nav>
          </header>
          <div class="container">
            <section id="hero">
              <h2><b>Handcrafted, home-made masterpieces</b></h2>
              <form action="https://www.freecodecamp.com/email-submit" id="form">
                <input type="email" id="email" placeholder="Enter your email address"  required>
                <input type="submit" id="submit" class="btn" value="GET STARTED">
              </form>
            </section>
            <section id="features">
              <div class="main_feature">
                <div class="icon"><i class="fa fa-3x fa-fire"></i></div>
                <div class="desc">
                  <h2>Premium Materials</h2>
                  <p>Our trombones use the shiniest brass which is sourced locally. This will increase the longevity of your purchase.</p>
                </div>
              </div>
              <div class="main_feature">
                <div class="icon"><i class="fa fa-3x fa-truck"></i></div>
                <div class="desc">
                  <h2>Fast Shipping</h2>
                  <p>We make sure you recieve your trombone as soon as we have finished making it. We also provide free returns if you are not satisfied.</p>
                </div>
              </div>
              <div class="main_feature">
                <div class="icon"><i class="fa fa-3x fa-battery-full"></i></div>
                <div class="desc">
                  <h2>Quality Assurance</h2>
                  <p>For every purchase you make, we will ensure there are no damages or faults and we will check and test the pitch of your instrument.</p>
                </div>
              </div>
            </section>
            <section id="How-It-Works">
              <iframe id="video" width="430px" height="200px" 
               src="https://www.youtube-nocookie.com/embed/y8Yv4pnO7qc?rel=0&controls=0&showinfo=0" >  </iframe>
            </section>
            <section id="Pricing" >
              <div class="price">
                <div class="card-head">
                  <h3>TENOR TROMBONE</h3>
                </div>
                <div class="card-content">
                  <h2>$600</h2>
                  <ul>
                    <li>Lorem ipsum.</li>
                    <li>Lorem ipsum.</li>
                    <li>Lorem ipsum dolor.</li>
                    <li>Lorem ipsum.</li>
                  </ul>
                  <div>
                    <button class="btn">SELECT</button>
                  </div>
                </div>
              </div>
              <div class="price">
                <div class="card-head">
                  <h3>BASS TROMBONE</h3>
                </div>
                <div class="card-content">
                  <h2>$900</h2>
                  <ul>
                    <li>Lorem ipsum.</li>
                    <li>Lorem ipsum.</li>
                    <li>Lorem ipsum dolor.</li>
                    <li>Lorem ipsum.</li>
                  </ul>
                  <div>
                    <button class="btn">SELECT</button>
                  </div>
                </div>
              </div>
              <div class="price">
                <div class="card-head">
                  <h3>VALVE TROMBONE</h3>
                </div>
                <div class="card-content">
                  <h2>$1200</h2>
                  <ul>
                    <li>Lorem ipsum.</li>
                    <li>Lorem ipsum.</li>
                    <li>Lorem ipsum dolor.</li>
                    <li>Lorem ipsum.</li>
                  </ul>
                  <div>
                    <button class="btn">SELECT</button>
                  </div>
                </div>
              </div>
            </section>
            <footer id="footer">
              <div id="footer-content">
                <div id="footer-link"> 
              <a href="#container">Privacy</a>
              <a href="#container">Terms</a>
              <a href="#container">Contact</a>
            </div>
                <div id="copy-right">
                  <p>Copyright 2016, Original Trombones</p>
                </div>
              </div>
            </footer>
          </div>
          </body>
          </html>


       


  ---
  
> ## 3. Functions, Methods, and Objects:
  
1. Functions: Functions consist of a In  series of statements that have been grouped together because they perform a specific task. 

2. Method: is the same as function, except methods are created inside (and are part of) an object.

3. Objects: programmers use objects a set of objects that act to create models of the like a toolkit for creating world using data, and that interactive web pages. objects are made up of This section introduces a properties and methods. you to a number of built-in In this section, you learn objects, which you will how to create your own then see used throughout

![Functions](https://miro.medium.com/max/852/1*DGzVYGrUe9yY46sGkuSlyg.png)

 ---
 
> ## 4. Pair Programming

![ Pair Programming](https://raw.githubusercontent.com/DXHeroes/knowledge-base-content/master/files/pair-programming.svg?sanitize=true)

* **Pair programming** is an agile software development technique in which two programmers work together at one workstation. One, the driver, writes code while the other, the observer or navigator, reviews each line of code as it is typed in. The two programmers switch roles frequently.


* **Why pair program?**

* There are six main reasons that indicates why is pair programming is very important:

 1. Greater efficiency: pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features
 
 2. Engaged collaboration: When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone
 
 3. Learning from fellow students: working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.
 
 4. Social skills: Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities.

 5. Job interview readiness: A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base
 
 6. Work environment readiness: Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a products
 
 


 

 
