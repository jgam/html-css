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
static : default place and be placed where we tell it to ex) just default 
fixed: no matter what goes to the specific place and on top of everyone ex) help chat bot
absolute: positioned based on relative(parent element) if not exist, then based on body ex) header menus
relative: parent element who wants to pass on child element some positionings ex) header

## flex
flex-direction: column, column-reverse, row, row-reverse
justify-content: center, space-between, space-around, flex-start, flex-end
align-items: center, flex-start, flex-end
align-self: center, flex-start, flex-end
order: value
flex-wrap: wrap(multiple lines), nowrap(one-line), wrap-reverse(multiple lines but reverse)
flex-flow: row,column wrap,wrap-reverse

## css selectors and pseudo selectors
input[required="required"]{

}
.box: first-child, last-child..{}
.box: nth-child(3n+2){}
input > .box{}

## css states
active (when clicked)
- .box:active{
    background-color: green;
}
focus (the strongest state and it focuses when it is being clicked with background color)
- .box:focus{
    background-color: blue
}
hover (when mouse is top of it)
- .box:hover{
    background-color: pink;
}
visited

## transitions
transition: changeable attributes in actions, time, effect
transition: background-color,all 5s ease-in-out;
You should put this in the tag ex) box

## transformations
transform: action(magnitude)
transform: rotate(20deg);

## animations
in the box you decalre: animation: 1.5s(time) scaleAndRotateSquare(the declared animation) ease-in-out(effect)
@keyframes(tells css that i created animations) scaleSquareRotateSquare(name of the animation) {
    from{
        transform:none
    }
    to{
        transform: rotate(1turn) scale(.5, .5);
    }
}

One thing to note is there can be many steps, only two is: from to, but more you can give percentage. 4 steps: 0 33 66 100, 5 stesps: 0 25 50 75 100

## Media queries
different browsers for big screen and small screens
body{
    background-color: green;
}
@media screen and (min-width:320px) and (max-width:640px){
    body{
        background-color: blue;
    }
}

for screen that is size between of width: 320px and 640px bgc will be blue otherwise, will be green.