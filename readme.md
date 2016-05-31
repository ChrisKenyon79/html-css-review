# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.
<!--

<!DOCTYPE>
<html>
<head></head>
<body></body>
</html>

-->

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
Explain here.
```
<!-- 
Image (or the alternate of the image) puts those items on the page. 
An empty div just puts a space between the items before and after
(vertical space) that can hold other stuff. Img can only hold images. 

-->

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Explain here

<!--
The first div with style uses css directly in the html. It won't
apply outside of the div. 

The second style tag uses the link to allow css to be used as 
it's own style sheet on this particular page. 
-->

```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.


div {
  border-radius: 50%;
}

/* border radius of 50% will make the framed item a circle.
as the selector (property type), it applies to all divs */



.header p {
  font-size: 18px;
}

/* this will make all Ps inside header (children of header named 'p')
have the font size of 18 pixels.   */



.footer {
  position: absolute;
  bottom: 0;
}

/* absolute position makes the element (footer) positioned relative to 
the original relative-positioned element previous to it. 
We NEED the relative positioned element to exist first, then
the absolute positioned element can use adjustments (top, right)
to move. 
Without the absolute pos element, the relative element simply 
uses the top of the page as the reference. 
*/



.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/*  Since the width is 100%, it will
stretch (or squeeze, NOT cut)the image horizontally. 



.ninja:hover {
  display: none;
  color: black;
}
```

/* hover will apply to all classes of "ninja". 
Hover looks at the mouse pointer position (it is hovering over the elem?)
and then enact the code - in this case, make it disappear (turn black)
*/