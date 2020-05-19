## Pseudo Classes

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
