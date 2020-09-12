# technical-documentation
<style>
  body{
  background-color:white;
  margin:0;
  padding:0;
}
#navbar{
  margin:0;
  padding:0;
  position:fixed;
  width:30%;
  height:100%;
  overflow:auto;
}
.nav-link{
  display:block;
  font-size:20px;
  color:black;
}
.nav-link:hover{
  background-color:lightgreen;
  height:50px;
  padding:5px;
}
#ul {
  list-style-type: none;
}
a:link{
  text-decoration:none;
}
#main-doc{
  margin-left:450px;
  height:auto;
}
#code{
  background-color:lightgray;
  padding:5px;
  width:50%;
}
.header{
  background-color:lightgreen;
  height:30px;
  padding:10px;
}
#img{
  width:100%;
}
@media screen and (max-width: 700px) {
  #navbar {
    width: 100%;
    height: auto;
    position: relative;
  }
  #navbar a {float: left;}
  #main-doc {margin-left: 0;}
  #img{
  width:50%;
}
}

@media screen and (max-width: 400px) {
  #navbar a {
    text-align: center;
    float: none;
  }
  #img{
  width:50%;
}
}
  </style>
<nav id="navbar">
  <ul id="ul">
<h1>CSS Documentation</h1><hr>
  
      <li><a class="nav-link" href="#css_intro">CSS Introduction</a></li><br><hr>
          <li><a class="nav-link" href="#css_syntax">CSS Syntax</a></li><br><hr>
          <li><a class="nav-link" href="#css_selectors">CSS Selectors</a></li><br><hr>
      <li><a class="nav-link" href="#css_comments">CSS Comments</a></li><br><hr>
          <li><a class="nav-link" href="#css_colors">CSS Colors</a></li><br><hr>
          <li><a class="nav-link" href="#css_backgrounds">CSS Backgrounds</a></li><br><hr>
    </ul>
  </nav>
<main id="main-doc">
  <section class="main-section">
    <h1  class="header" id="css_intro">CSS Introduction</h1>
    <h4>What is CSS?</h4>
    <ul>
      <li>CSS stands for Cascading Style Sheets</li>
      <li>CSS describes how HTML elements are to be displayed on screen, paper, or in other media</li>
      <li>CSS saves a lot of work. It can control the layout of multiple web pages all at once</li>
      <li>External stylesheets are stored in CSS files</li>  
    </ul>
    <h4>Why used CSS?</h4>
    <p>CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.</p>
    <strong><p>CSS Example</p></strong>  
    <p id="code">
body <br>{<br>
  background-color: lightblue;<br>
}
<br>
h1 <br>{<br>
  color: white;
  text-align: center;<br>
}
<br>
p<br> {<br>
  font-family: verdana;
  font-size: 20px;<br>
}</p>
  </section>
  <section id="main-section"> 
  <h1 class="header" id="css_syntax">CSS Syntax</h1>
    <p>A CSS rule-set consists of a selector and a declaration block:</p>
    <img id="img" src="https://www.w3schools.com/css/selector.gif" alt="syntax">
    <p>The selector points to the HTML element you want to style.</p>
     <p>The declaration block contains one or more declarations separated by semicolons.</p>
     <p>Each declaration includes a CSS property name and a value, separated by a colon.</p>
     <p>Multiple CSS declarations are separated with semicolons, and declaration blocks are surrounded by curly braces.</p>
    <strong><p>Example</p></strong>
    <p>
In this example all elements will be center-aligned, with a red text color:</p>
    <p id="code"> p <br>{<br>
  color: red;
  text-align: center;<br>
}</p>
    <strong><p>Example Explained</p></strong>
      <ul>
        <li>p is a selector in CSS (it points to the HTML element you want to style: <p>).</li>
         <li>color is a property, and red is the property value</li>
         <li>text-align is a property, and center is the property value</li>
      </ul>
  </section>
  <section id="main-section">
    <h1 class="header" id="css_selectors">CSS Selectors</h1>
    <p>CSS selectors are used to "find" (or select) the HTML elements you want to style.</p>
    <p>We can divide CSS selectors into five categories:</p>
    <ul>
      <li>Simple selectors (select elements based on name, id, class)</li>
       <li>Combinator selectors (select elements based on a specific relationship between them)</li>
       <li>Pseudo-class selectors (select elements based on a certain state)</li>
       <li>Pseudo-elements selectors (select and style a part of an element)</li>
       <li>Attribute selectors (select elements based on an attribute or attribute value)</li>
    </ul>
  </section>
  <sectio id="main-section">
    <h1 class="header"id="comments">CSS Comments</h1>
    <p>Comments are used to explain the code, and may help when you edit the source code at a later date.</p>
    <p>Comments are ignored by browsers.</p>
<p>A CSS comment is placed inside the style element, and starts with /* and ends with */:</p>
  <strong><p>Example</p></strong>
    <p id="code">/* This is a single-line comment */<br>
p<br> {<br>
  color: red;<br>
}</p>
  </section>
  
  <section id="main-section">
    <h1 class="header" id="css_colors">CSS Colors</h1>
    <p>
Colors are specified using predefined color names, or RGB, HEX, HSL, RGBA, HSLA values.</p>
    <strong><p>CSS Color Names</p></strong>
    <p>
In CSS, a color can be specified by using a color name:</p>
    <p style="background-color:tomato; width:50%;">Tomato</p>
    <p style="background-color:orange; width:50%;">Orange</p>
    <p style="background-color:dodgerblue; width:50%;">DodgerBlue</p>
    <p style="background-color:mediumseagreen; width:50%;">MediumSeaGreen</p>
    <p style="background-color:gray; width:50%;">Gray</p>
    <p style="background-color:slateblue; width:50%;">SlateBlue</p>
    <p style="background-color:violet; width:50%;">Violet</p>
    <p style="background-color:lightgray; width:50%;">LightGray</p>
    <strong><p>Example</p></strong>
    <p id="code">p <br> { <br>color:tomato;<br>}</p>
  </section>
  
  <section id="main-section">
    <h1 class="header" id="css_backgrounds">CSS Backgrounds</h1>
    <p>The CSS background properties are used to define the background effects for elements.</p>
    <p>In these chapters, you will learn about the following CSS background properties:</p>
    <ul>
      <li>background-color</li>
      <li>background-image</li>
      <li>background-repeat</li>
      <li>background-attachment</li>
      <li>background-position</li>
    </ul>
    <strong><p>Example</p></strong>
    <p>Here, the h1 tag, p tag, and div tag elements will have different background colors: </p>
    <p id="code">h1{<br>
  background-color: green;<br>
}<br>

div {<br>
  background-color: lightblue;<br>
}<br>

p {<br>
  background-color: yellow;<br>
}</p>
  </section>
  
  <section id="main-section">
    <h1 class="header" id="reference">Reference</h1>
    <p>All the documention is taken from <a href="https://www.w3schools.com/css/default.asp" target="_blank">W3Schools</a></p>
  </section>
</main> 
