# SO... what is HTML:




## First we need to dive into why it was invented:
before the creation of the internet as we know it,
there was a time where people were sharing text with each other.
in the early stages of the internet, imagine just showing a text file in place of the current standards of websites.

people back then didn't have the ability to "customize" their content which was plain text.


so they made a language that was just like how you piece different pieaces of LEGOs together to create something nice, they had the idea of making anything a block, that can either contain a text or image or even another block.

these blocks had default styles and names, for organization's sake.
there's:
- **div** which is a generic block
- **body** is the top block (under the document block)

there are some trict blocks for certian tasks,
for example
- **ol** and **li** for listing items
- **a** for links (it can't have a block inside it, it can but the browser will scream at ya)


### so what HTML actually is:
it's a short name for HyperText markup language,
HyperText, what is it,
it sounds like superText.. a future marvel movie? netflix take notes,

it just put things together and organize and group stuff in a blocky way,
it can also show text, images and import additional languages that could manipulate that DOM(just a fancy word of saying the current page and stuff within it).





## i think that's enough of that, let's talk about the syntax:
it's pretty simple
```html
<name_of_the_block  attribute_name="value_for_that_attribute">
content
</name_of_the_block>
```
does it seem complicated ...
let's break it down even further
so between the first <> there lies our customization for that block which are the attributes or you can call them properties.

lets talk logically, imagine you have a towel, what do you say about it, how do you describe its shape and look, what are the selling **attribute**, ex: 
it has a red color. it was a width and height of 40cm.
- color is an attribute of value "red"
- width same thing with value of "40cm", same thing with height

so it will look like this
```html
<towel color="red" width="40cm" height="40cm">made in china</towel>
```

**note:** i lied.. the color is not a attribute, not in HTML default components...
for a good reason, we will know why there isn't a color atribute later when we talk about css

we will use the attribute `class` for like .. everything... so 











