[CodePen](https://codepen.io/pen)

#### Adding Media to a Web Page ####
Example: lesson_index.html

#### List ####
1. Unordered list 
2. Ordered list 
3. Description list 
  
#### Bold & Italic ####

#### special characters ####
Right single quote: ’
Left single quote: ‘
Right double quote: ”
Left double quote: “
Ampersands: &
Greater than: >
Less than: <
Copyright: ©
Registered symbol: ®
Trademark symbol: ™

#### Semantic Structural Elements ####
"<header>" "<footer>" "<article>"
  + header, footer are in article
 "<aside>"

#### navigation ####
Example: Nav

#### Non-semantic Elements ####
"<div> division/section || block-level" <br/>
 "<div class="">" <br/>
"<span> sepate words || inline" <br/>
 "<span class="">"
  
#### HTML Comments ####
"<!-- This is where the main text of the article begins -->"

#### The Section Element ####
"<section> || chapter"<br/>
"section in section - subsection"
  
#### Forms ####
+ basic type of forms
+ different type of inputs
     - email, tel, textarea
+ choosing between a set of options
     - Select (dropdown)
     - Radio
     - Checkbox

#### Tables ####
Example: table.html

#### CSS Essentials ####
##### CSS Selectors ######
1. Type selectors
2. Descendant selectors
3. Class selectors
##### The Cascade ######
+ The Cascade
+ Inheritance
+ Specificity
##### CSS Box Model #####  
##### Layout with float #####  
##### Beauty School #####  

### Intermediate CSS ###
##### Styling Navigation Menu #####  
##### Position Relative Absolute ##### 
position: absolute/ relative;<br/>
z-index: stacking overlap<br/>


### Necessary CSS Tasks ###
##### Styling Data Tables ##### 
Example: table style
##### Styling Forms ##### 
[formalize.css](https://formalize.me)<br/>
[normalize.css](http://necolas.github.io/normalize.css/)<br/>
Example: form style

### CSS Typography ###
font-family: 为段落设置字体<br/>
##### Using Custom "Web" Fonts #####
1. Hosted Font Solutions
     - Adobe TypeKit (paid)
     - Google Fonts (free)
2. Self Hosted Fonts
     - @font-face

### Developer Timeout! ###
##### Developer Tools | Inspect Elements #####
1. Tracking down where properties are coming from
2. Experimenting or troubleshooting
3. Inspiration from other websites

### CSS Backgrounds ###
##### Background Images #####
example1: <br/>
background-image: url(../images/color-tile.png); <br/>
background-repeat: repeat-x;

example2: <br/>
background-image: url(../images/flower.jpg); <br/>
background-position: right center;<br/>
background-repeat: no-repeat;

example3:<br/>
background: #c2bbb1 url(../images/bird.jpg) center center no-repeat;<br/>
background-size: cover;<br/>

example4:<br/>
background: url(../images/color-tile.png) left bottom repeat-x, #FFF url(../images/color-tile.png) left top repeat-x;

##### Gradient Background #####
example1:<br/>
background-color: #e5e9dc;<br/>
background-image: -webkit-gradient(linear, left top, left bottom, from(#e5e9dc), to(#FFF));<br/>
background-image: -webkit-linear-gradient(top, #e5e9dc, #FFF);<br/>
background-image: -moz-linear-gradient(top, #e5e9dc, #FFF);<br/>
background-image: -ms-linear-gradient(top, #e5e9dc, #FFF);<br/>
background-image: -o-linear-gradient(top, #e5e9dc, #FFF);<br/>
background-image: linear-gradient(to bottom, #e5e9dc, #FFF);<br/>

##### CSS Sprites #####
what, Why, How to use CSS Sprites 
+ Used for "icon" art
+ Reduces number of HTTP requests
+ CSS recipe: "background-image" & "background-position"
+ [GIMP](gimp.org) &nbsp; (Photoshop Alternative)
Example: Sprites file

##### Full Width Backgrounds - Fixed Width Content #####
example1:<br/>
max-width: 940px;<br/>
margin: 0 auto;<br/>
padding-left: 40px;<br/>
padding-right: 40px;<br/>

### Responsive Web Design ###
##### Responsive Web Design #####
Our Responsive Recipe
1. Meta tag in head section of HTML
      - meta nam="viewport" content="width=device-width, initial-scale=1" (no change)
2. Media queries (conditional CSS)
      - @media screen and (max-width: 480px)
      - class="info-box hide-small" (2 classes: info-box, hide-small)
      - @media screen and (min-width: 1300px)

##### Responsive Grids #####
1. What is a grid?
2. What is a responsive grid?
3. How can we code a grid?

+ Viewport Size Abbreviations
      - xs = Extra Small (smartphones)
      - sm = Small (tablet) 
      - md = Medium (laptop or medium monitor) 
      - lg = Large (desktop large monitor)
     
### CSS3 Special Effects ###
##### Box Shadows #####
example1: <br/>
box-shadow: 10px 2px 5px #000# <br/>
example2: <br/>
box-shadow: inset 10px 5px 5px 5px rgba(0,0,0, .15);<br/>
example3: <br/>
box-shadow: inset 3px 3px 5px rgba(0, 0, 0, .33), 10px 5px 5px rgba(0, 0, 0, .15);

##### Rounded Corners #####
example1:<br/>
border-radius: 10px 25px; <br/>
example2:<br/>
border-radius: 10px 10px 25px 25px; <br/>
example3(unique shape):<br/>
border-radius: 10px/25px; <br/>
example4:<br/>
border-radius: 10px; <br/>
example5:<br/>
bborder-radius: 50%; <br/>

##### CSS Transform #####
Transform Big Four
1. Rotate 
example: <br/>
transform: rotate(15deg);<br/>
2. Scale <br/>
example: <br/>
transform: scale(1.5)<br/>
3. Skew<br/>
example1: <br/>
transform: skewX(25deg);<br/>
example2: <br/>
transform: skewY(-25deg);<br/>
example3: <br/>
transform: skewY(-25deg) skewX(15deg);<br/>
4. Position (origin & placement)<br/>
example1: <br/>
transform-origin: 100% 0;<br/>
example2: <br/>
transform: translateX(100px) translateY(50px);<br/>
example3: <br/>
transform: translate(100px, 50px);<br/>
example4: <br/>
position: relative;<br/>
top: 50px;<br/>
left: 100px;<br/>
+ position: relative vs translate()
      - Layout purpose = Use position: relative (Not Hardware-accelerated)
      - Animation purposes = Use translate() (Hardware-accelerated)

##### CSS Transitions #####
example1: <br/>
transition-property: color, background-color / all; <br/>
transition-duration: 2s; <br/>
example2: <br/>
transition: all 1s;<br/>
transition-timing-function: ease-in-out;<br/>

##### CSS Animations #####
example1: <br/>
@Keyframes fadeBounce {}<br/>
0% {opacity: 0; transform: translateY(-200%)}; <br/>
45%{}, 55%{}, 75%{} <br/>
100% {opacity: 1; transform: translateY(0)}; <br/>
<br/>
animation-name: fadeBounce; <br/>
animation-duration: 1s; <br/>
<br/>
opacity: 0; <br/>
animation-fill-mode: forwards <br/>
<br/>
.boxes :nth-child(2) .box-a {animation-delay: .5s;} <br/>
example2: <br/>
animation: fadeBounce 1s forwards; <br/>
example3: <br/>
@-webkit-Keyframes slideSpin {} <br/> 
-webkit-animation: <br/> 
50% {transform: translateX(150%) scale(.5);} <br/>
75% {transform: translateX(150%) rotate(180deg) scale(.5);} <br/>
100% {transform: translateX(300%) rotate(180deg);} <br/>
<br/>
animation: slideSpin 2s; <br/>
animation-fill-mode: forwards; <br/>
animation-iteration-count: infinite; <br/>
animation-direction: alternate; <br/>

### Leveraging JavaScript without Writing JavaScript ###
##### Slideshow (part I) ##### 
Recipe for a Slideshow:
+ Our own HTML & CSS
+ Cycle2 by Mike Alsup
<br/>
script type="text/javascript" src="js/cycle2.js"
<br/>
Dependency jQuery <br/>
script type="text/javascript" src="js/jquery.js" <br/>
class="cycle-slide" <br/>
class="slide" class="slide-text" <br/>
div class="cycle-slideshow" data-cycle-slides=".slide/img/.item" <br/>
/* Slideshow Styles */ <br/>
/* Prev and Next Buttons */  <br/>

##### Slideshow (part II) ##### 

##### Reveal & Hide Content on Click/Tap ##### 
Our Recipe:
+ Custom HTML & CSS
+ JavaScript: Declarative Toggle
<br/>
script type="text/javascript" src="js/declarativeToggle.js" <br/>
span data-toggle-target=".site-nav" class="toggle-btn" <br/>
/* Reveal and Hide Styles */ <br/>

#####  Open Image in Modal Window(Gallery) ##### 
Our Recipe:
+ Custom HTML & CSS
+ Lightbox by Lokesh Dhakar
<br/>
link rel="stylesheet" href="css/lightbox.css" <br/>
script type="text/javascript" src="js/lightbox.min.js" <br/>
data-lightbox="gallery" <br/>
Find: ../img/ -> Replace: ../images/ <br/>
/*thumbnails (img) hover*/ <br/>




### Popular Communities ###
+ WordPress
+ Drupal
+ Ruby on Rails
+ Symfony
+ CodeIgniter
