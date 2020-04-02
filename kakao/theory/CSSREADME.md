# CSS

## Selector and property
CSS has two parts: selector and property.

h1 {//this is selector

    property-name: value; // this is property

}

class = .classname
id = #id
general tag = general tag

## inline css and why is it bad?
In order to connect the HTML file and css file, inline CSS is one way. What you can do is, in your html, you can open <styles></styles> tag and put whatever styling u want in there.

The problem is though, we may have multiple index files and if we want to apply same stylings, we have to go each of them and correct it.

This is very timestaking and inefficient. So we can call it by importing external css file with <link href="styles.css" rel="stylesheet">

## box model
content - real content in the box
border - the border of the box we created
padding - inside space of border, space between border and content
margin - outside space of border, space between border and outside

## inline block
Box does not allow any elements next to it which means it cannot be flexed or inlined.

However, if u use, inline-block, then depending on the width, it will allow next box to allign with the previous ones. However, display inline will erase all the css before and adjust to the content of the tag. so the property of box which is to not allow any thing aligning is gone.

display: box
diaplay :inline-box
display: inline ....<span>1</span>

## Position property

