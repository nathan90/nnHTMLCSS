# HTML and CSS
## 1. Introduction

- HTML is a Hypertext Markup Language used to structure content on a web page.
- We structure content using HTML tags.
```html
          <html>
            <body>
              <p> Content </P>
              <a> link </a>
            </body>
          </html>
 ```

 ## 2.  HTML Basics
 
 ### HTML Tags

  - `<!DOCTYPE>`  	Defines the document type.
  - `<html>` 	Defines an HTML document.
  - `<head>` 	Contains metadata/information for the document.
  - `<body>` 	Defines the document's body.
  - `<h1> to <h6>` 	Defines HTML headings. `h1` the largest to `h6` the smallest
  - `<p>` 	Defines a paragraph tag.
  - `<br>` 	Inserts a line break.
  - `<blockquote>` 	Defines a section that is quoted from another source.
  - `<a>`	Defines a hyperlink. Used for inserting urls to other sites or same site
  - `<em>` 	Defines emphasized text. Usually in italics
  - `<strong>` Defines text in bold
  - `<form>` 	Defines an HTML form for user input.
  - `<label>` 	Defines a label for an <input> element.
  - `<input>` 	Defines an input control.
  - `<select>`	Defines a drop-down list.
  - `<button>` 	Defines a clickable button.
  - `<img>`	Defines an image.
  - `<ul>` 	Defines an unordered list.
  - `<ol>` 	Defines an ordered list.


## 6 - HTML Semantic Tags

* \<main> - For the main content of a web page
* \<section> - Defines a certain section of a web page (eg. blog list, contact info)
* \<article> - Defines a bit of the content which makes up an article(eg a blog post)
* \<aside> - Defines some content related to something else (eg: similar blog posts)
* \<header> - For the header of a website - contains the nav, title etc
* \<footer> - For the footer of a website - contact information, copyright notice etc

## 8 - CSS Layout and Position

Static, Fixed, Relative, Absolute, Sticky
We use these to position elements differently on a page

### Static
It is the default value

### Relative
if we fix an elements position to be relative we can shift it relative to its original position  
The space it was originally in will be retained
```
{  
    position: relative;  
    left: 20px;  
    bottom: 20px;  
}  
```

### Fixed

Positions a certain element relative to the viewport  
Viewport is part of web browser that we see the web page on  
for example in the case of a navigation bar  
```{  
    position: Fixed  
    left: 0px  
    right: 0px  
}  
```
even when we scroll down the nav bar remains at the top  

### Absolute

Absolute allows us to position things absolutely relative to its closest parent which is also given  
a position property that is not static.  
```
{  
    position: absolute  
    left: 20px  
    bottom:20px  
}  
```
When we use absolute on any tag the rest of the content will move up. When we position something  
absolutely, we take it out of normal document flow and we lose that space that it was originally in

### Sticky

It is a mixture of static and fixed. A sticky element toggles between relative and fixed, depending on the  
scroll position. It is positioned relative until a given offset position is met in the viewport - then it  
sticks in place like position:fixed

## 9 - Pseudo Classes

They are special keywords we can use in CSS and add to selectors so we can target elements when they are in a particular state. eg when we hover over an element, when an form field is in focus, when an element is the first child of the parent element. We use pseudo classes by tagging them on to the end of css selector with a colon and keyword :keyword  

Some of the keywords are  
* **hover** which does some element manipulation when mouse is hovered over the element
* **focus** which does element manipulation when an element is selected for eg selecting an input field
* **valid** which does element manipulation for example if the user enters the correct email in its field
* **first-child** tag the child of a parent element when it the first child inside that parent element

For further reference: https://www.w3schools.com/css/css_pseudo_classes.asp

## Pseudo Elements

Pseudo elements allows us to inject dynamic content. Its syntax is  selector::pseudo-element {}
Some of the pseudo elements are  
* ::after - Insert something after the content of each \<p> element
* ::before - Insert something before the content of each \<p> element
* ::first-letter - Selects the first letter of each \<p> element
* ::first-line - Selects the first line of each \<p> element
* ::selection - Selects the portion of an element that is selected by a user

For further reference: https://www.w3schools.com/css/css_pseudo_elements.asp

## 10 - Media Queries and Responsive Design

**Media Queries** tell the browser how to style an element at particular viewport dimensions
**Viewport Meta Tag** tells the browser what width the viewport should be
**Responsive Images** Only load smaller images for mobile devices

In practice when designing a project approach a mobile first approach. plan our site for a small mobile device first and scale it to larger screen. Prioritize around important content

For further reference: https://www.w3schools.com/css/css_rwd_viewport.asp


#### Next to do
CSS FlexBox