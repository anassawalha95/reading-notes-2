> # Class 02 *Jan 04 2021:*

> ## Topics

   1. Text
    
   2. Introducing CSS
    
   3. Basic JavaScript Instructions
    
   4. Decisions and Loops
    
   
---

> ## 1. Text

* There are two main HTML Tags:

   1. Structural Markup: the elements that you can use to describe both headings and paragraphs
   
   2. Semantic markup: which provides extra information; such as where emphasis is placed in a sentence
   
* Some Semantic tags: 
    
   1. Heading `<h1>-<h6>`
   
         `<h1>`: Used for Headings 
   
        `<h2>-<h6>`: Used for Subheading
   
   2. Paragraph `<p>`: To create a paragraph
   
   3. Bold `<b>`: for bold text
   
   4. Italic `<i>`: for italic text
       
   5. Suberscript & Subscript: The `<sup>` element is used to contain characters that hould be superscript such as the suffixes of dates or mathematical concepts, The `<sub> `element is used to contain characters that should be subscript.
   
   6. Line Breaks `<br>`
   
   7. Horizontal Rules `<hr>`
   
   8. Strong ` <strong> `: The use of the `<strong>` element indicates that its content has strong importance. 
   
   9. Emphasis ` <em> ` : The `<em>` element indicates emphasis that subtly changes the meaning of a sentence. 
   
   10. Quotations `<blockquote>`: The `<blockquote>` element is used for longer quotes that take up an entire paragraph.
   
   11. Abbreviations `<abbr>`: If you use an abbreviation or an acronym, then the `<abbr>` element can be used.
   
   12. Citations `<cite>`: When you are referencing a piece of work such as a book, film or research paper, the `<cite>` element can be used to indicate where the citation is from.
   
   13. Definition `<dfn>`: The first time you explain some new terminology (perhaps an academic concept or some jargon) in a document, it is known as the defining instance of it.
   
   14. Author Details `<address>`: The <address> element has quite a specific use: to contain contact details for the author of the page.
   
   15. `<ins>` `<del>`: The `<ins>` element can be used to show content that has been inserted into a document, while the `<del>` element can show text that has been deleted from it.
   
   16. The `<s>` element indicates something that is no longer  accurate or relevant (but that should not be deleted).
   
---
   

> ## 2. Introducing CSS

* **CSS Stand for:** cascading style sheet that allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

* **You can use CSS in three ways:**
   
   1. by adding the styles in the head tag useing style tag
   
   2. by adding the style tag attribute. EX: `<p style=" color: red">`
   
   3. by including the style from another file  EX: `<link href="css/styles.css" type="text/css" rel="stylesheet" />`
   
* some css Properties:

  1. width
  
  2. height
  
  3. border
  
  4. shadow
  
  5. color
  
![css rule](https://puzzleweb.ru/en/images/css/1_1.png)

Example:


         body {
         font-family: Arial, Verdana, sans-serif;}
         h1, h2 {
         color: #ee3e80;}
         p {
         color: #665544;}
---

> ## 3. Basic JavaScript Instructions
  
* **Javescript**: is used to create actions or events in webpages

* **Comments** use `//` or `/* */` for comments 

* **Variables**: Use the `var` to define variables in JS to store values for  example: `var likes = 10;`. It have three value types:
   
   1. number
   
   2. string
   
   3. boolean
   
    
* **Arrays**:  An array is a special type of  a variable it dosen't store one value only it stores  a list of values 
![arrays](https://miro.medium.com/max/2008/1*UPZgcwkDOCQbzWIuEqHD9w.jpeg)
---

> ## 4. Decisions and Loops

* **There are There Three Main Concepts to Determine The Path in to Take in Programmin:**

1. Evaluations: Analyze values in you scripts to determine whethere or note match expected results 

2. Decisions: Using the results of evaluations, you can decide which path your script should go down. 

3. Loops: There are also many occasions where you will want to perform the same  set of steps repeatedly.


Examples: 
  
**LOOP:**

![loop](https://cdn.programiz.com/sites/tutorial2program/files/javascript-while-loop.png)

**If statment**

![if statment](https://cdn.javascripttutorial.net/wp-content/uploads/2016/08/JavaScript-if-statement.png)

**Logical Operators**
| NAME                    | OPERATOR | PURPOSE & NOTES                                                  |
|-------------------------|:--------:|------------------------------------------------------------------|
| Is Equal To             |    ==    | Compare value true if are equal                                  |
| Is Not Equal To         |    !=    | Compare value true if are not equal                              |
| Strict Equal To         |    ===   | Compare value and type true if are equal                         |
| Strict Not Equal To     |   !===   | Compare value and type false if both aren't equal                |
| Grater Than             |     >    | Checks if number on the left greater than on the right           |
| Less Than               |     <    | Checks if number on the left less than on the right              |
| Grater Than or Equal To |    >=    | Checks if number on the left greater than or equal on the right  |
| Less Than or Equal To   |    <=    | Checks if number on the left less than or equal on the right     |
