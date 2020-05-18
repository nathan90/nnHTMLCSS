## CSS Layout and Position

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
