> # Class 14a *Jan 20 2021:*

> ## Topics

  1. Build the Perfect Team 

  2. CSS Transform [Referance]

  3. CSS Transitions & Animations 
  
  
---
 
> ## 1. Build the Perfect Team [Referance](https://www.google.com/amp/mobile.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.amp.html)

![team work](https://i.dlpng.com/static/png/4149988-hands-connecting23-2147506270-annual-giving-network-connecting-hands-png-456_458_preview.webp)

* **Summary:**

The writter Introduced Julia Rozvosky where she started as student at Yale unversity and worked in different sectors that she didn't like. After that she found her passionate job as Aristotle's researcher at google. 

Rozovsky studied thousand of reserches to find the best build for a perfect team at google where she collected a study results out of 699 contribuoter in her study. after that she found out that the best team build is to have a straight forward manager who creates a clear guidline for his team members.
 
After that Rozvoky met with Matt Sakaguchi who was athletic and got hired as middleware mananger and he contributed in finding the best build for a perfect team by adding that: team members should open up about thier struggles which is very criticl to success of the team and creates awreness, resillance, and teams member exscuses each other on upnormal condtions.


----

>##  2. CSS Transform [Referance](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

![CSS Transform](https://speckyboy.com/wp-content/uploads/2017/11/css-2.jpg)

* **With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.**

* **The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.**

---- 

#### 1. 2D Transforms:

   1. 2D Rotate: The rotate value provides the ability to rotate an element from 0 to 360 degrees.

            .box-1 {
                transform: rotate(20deg);
            }
                .box-2 {
                transform: rotate(-55deg);
            }

   2. 2D Scale: allows you to change the appeared size of an element. 

            .box-1 {
                transform: scale(.75);
                }
                .box-2 {
                transform: scale(1.25);
            }

   3. 2D Translate: works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, followed by a comma, and then the y axis value.

            .box-1 {
                 transform: translateX(-10px);
            }
            .box-2 {
                transform: translateY(25%);
            }
            .box-3 {
                transform: translate(-10px, 25%);
            }

   4. 2D Skew: used to distort elements on the horizontal axis, vertical axis, or both.

            .box-1 {
                transform: skewX(5deg);
            }
            .box-2 {
                transform: skewY(-20deg);
            }
            .box-3 {
                transform: skew(5deg, -20deg);
            }

   5. Transform Origin: the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. 

            .box-1 {
                transform: rotate(15deg);
                transform-origin: 0 0;
            }
            .box-2 {
                transform: scale(.5);
                transform-origin: 100% 100%;
            }
            .box-3 {
                transform: skewX(20deg);
                transform-origin: top left;
            }
            .box-4 {
                transform: scale(.75) translate(-10px, -10px);
                transform-origin: 20px 50px;
            }


   6. Perspective: work the elements need a perspective from which to transform

        .box {
            transform: perspective(200px) rotateX(45deg);
        }

----

#### 2. 3D Transforms:

   1. 3D Rotate: allows you to rotate an element around the x axis, as if it were being bent in half horizontally. Using the rotateY value allows you to rotate an element around the y axis, as if it were being bent in half vertically. Lastly, using the rotateZ value allows an element to be rotated around the z axis.

          .box-1 {
              transform: perspective(200px) rotateX(45deg);
          }
          .box-2 {
              transform: perspective(200px) rotateY(45deg);
          }
          .box-3 {
              transform: perspective(200px) rotateZ(45deg);
          }

   2. 3D Scale: By using the scaleZ three-dimensional transform elements may be scaled on the z axis.

          .box-1 {
              transform: perspective(200px) scaleZ(1.75) rotateX(45deg);
          }
          .box-2 {
              transform: perspective(200px) scaleZ(.25) rotateX(45deg);
          }

   3. 3D Translate : elements may also be translated on the z axis using the translateZ value. 

          .box-1 {
              transform: perspective(200px) translateZ(-50px);
          }
          .box-2 {
              transform: perspective(200px) translateZ(50px);
          }

----

#### 3. Backface Visibility

* **When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. This may be caused by setting the rotateY(180deg) value for example. By default these elements are shown from the back. So if you prefer not to see these elements at all, set the backface-visibility property to hidden, and you will hide the element whenever it is facing away from the screen.** 

        .box-1 {
            transform: rotateY(180deg);
        }
        .box-2 {
            backface-visibility: hidden;
            transform: rotateY(180deg);
        }


----

#### 3. CSS Transitions & Animations: [Referance](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

* **Transitional Properties:** The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change.

| background-color | background-position |  border-color  |
|:----------------:|:-------------------:|:--------------:|
|   border-width   |    border-spacing   |     bottom     |
|       clip       |        color        |      crop      |
|     font-size    |     font-weight     |     height     |
|       left       |    letter-spacing   |   line-height  |
|      margin      |      max-height     |    max-width   |
|    min-height    |      min-width      |     opacity    |
|   outline-color  |    outline-offset   |  outline-width |
|      padding     |        right        |   text-indent  |
|    text-shadow   |         top         | vertical-align |
|    visibility    |        width        |  word-spacing  |
|      z-index     |                     |                |

                HTML

            <div class="stage">
            <figure class="ball"></figure>
            </div>

                        
                CSS

            @keyframes slide {
            0% {
                left: 0;
                top: 0;
            }
            50% {
                left: 244px;
                top: 100px;
            }
            100% {
                left: 488px;
                top: 0;
            }
            }
            .stage {
            height: 150px;
            position: relative;
            }
            .ball {
                height: 50px;
                position: absolute;
                width: 50px;
            }
            .stage:hover .ball {
            animation-name: slide;
            animation-duration: 2s;
            animation-timing-function: ease-in-out;
            animation-delay: .5s;
            }

----

#### Side Projects to View:

**6 Buttons animated [Link](http://codepen.io/retyui/pen/ByoaXV)**


**CSS3 Animations: Keyframes [Link](http://codepen.io/akshaychauhan/pen/oAfae)**



**404 [Link](http://codepen.io/kieranfivestars/pen/MYdQxX)**



**Pure CSS Bounce Animation [Link](http://codepen.io/dp_lewis/pen/gCfBv)**


----



Github Live: [view](https://anassawalha95.github.io/reading-notes-2/Class%2014a)

Github Repo: [view](https://github.com/anassawalha95/reading-notes-2/blob/main/Class%2014a.md)
