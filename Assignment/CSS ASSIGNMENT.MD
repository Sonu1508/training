# CSS ASSIGNMENT

## Q.1.What is CSS?
ANS:CSS stands for Cascading Style Sheet. It’s a style sheet language that determines how the elements/contents in the page are looked/shown. CSS is used to develop a consistent look and feel for all the pages.
CSS was developed and is maintained by the World Wide Web Consortium (W3C). It was first released on December 17, 1996. The CSS Working group currently working with different browser vendors to add/enforce the new feature/ specifications in all the browsers.
CSS enables the separation of the content from the presentation. This separation provides a lot of flexibility and control over how the website has to look like. This is the main advantage of using CSS.
CSS3 or Cascading Style Sheets Level 3 is the third version of the CSS standard that is used to style and format web pages. CSS3 incorporates CSS2 standard with some improvements over it. The main change in CSS3 is the inclusion of divisions of standards into different modules that makes CSS3 easier to learn and understand. Learn More.

## Q.2. What are the advantages of using CSS?
The main advantages of CSS are given below:

- Separation of content from presentation - CSS provides a way to present the same content in multiple presentation formats in mobile or desktop or laptop.
- Easy to maintain - CSS, built effectively can be used to change the look and feel complete by making small changes. To make a global change, simply change the style, and all elements in all the web pages will be updated automatically.
- Bandwidth - Used effectively, the style sheets will be stored in the browser cache and they can be used on multiple pages, without having to download again.


## Q.3.What are the different types of Selectors in CSS?
ANS:A CSS selector is the part of a CSS ruleset that actually selects the content you want to style. Different types of selectors are listed below.

Universal Selector: The universal selector works like a wildcard character, selecting all elements on a page. In the given example, the provided styles will get applied to all the elements on the page.

* {
  color: "green";
  font-size: 20px;
  line-height: 25px;
}</br>
Element Type Selector: This selector matches one or more HTML elements of the same name. In the given example, the provided styles will get applied to all the ul elements on the page.</br>

ul {
  line-style: none;
  border: solid 1px #ccc;
}</br>
ID Selector: This selector matches any HTML element that has an ID attribute with the same value as that of the selector. In the given example, the provided styles will get applied to all the elements having ID as a container on the page.

#container {
  width: 960px;
  margin: 0 auto;
}</br>

<div id="container"> </div>
Class Selector: The class selector also matches all elements on the page that have their class attribute set to the same value as the class.  In the given example, the provided styles will get applied to all the elements having ID as the box on the page. </br>

.box {
  padding: 10px;
  margin: 10px;
  width: 240px;
}</br>

<div class="box"></div>

## Q.4.How do you specify units in the CSS?. What are the different ways to do it?
ANS:There are different ways to specify units in CSS like px, em, pt, percentage (%). px(Pixel) gives fine-grained control and maintains alignment because 1 px or multiple of 1 px is guaranteed to look sharp. px is not cascade. em maintains relative size. you can have responsive fonts. Em, will cascade 1em is equal to the current font-size of the element or the browser default. If u sent font-size to 16px then 1em = 16px. The common practice is to set default body font-size to 62.5% (equal to 10px).

pt(point) are traditionally used in print. 1pt = 1/72 inch and it is a fixed-size unit.

%(percentage) sets font-size relative to the font size of the body. Hence, you have to set the font-size of the body to a reasonable size.
