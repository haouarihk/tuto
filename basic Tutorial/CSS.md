## CSS:
Cascading Style Sheets also most known as a style sheet language

in simple terms it applies customization and description to a document(the page).

## syntax: 
```css
a way of selecting an item {
  property_name: your_value_for_it;

  /** example: */
  background: "pink";
  /** ...other properties here **/
}
```
The thing about css, it needs a way to select items, elements or blocks that it want to put your description on,
they came up with a way, multiple actually

- ### by id:
with id, you can only have one element (i usually avoid using it, because it makes a less reuseable code) you just basically just give attribute id and give it any **unique** name:
```html
<div id="imunique"></div>
```
```css
#imunique{
   background: "silver"
}
```
any description will only apply to one unique element of the same id


- ### by class:
now for the most commonly used
this allowes to select any element that has the class you're describing:

ex: you have the human class and intelegent
a person can be in the human class and intelegent class at the same time, that's the beauty of classes, 
```css
.human{
 color:"white";
}

.intelegent{
 width: "420cm";
}

```
```html
<person class="human intelegent"></person>
<dummy class="human"></dummy>
<alien class="intelegent"></alien>
```


- ### by name:
name of the element (ex: div, body, html... etc)
```css
name { }
```
any description will apply to all elements with the same name



### notes:
have you noticed that, to select using an id you put a hashtag before the id,
and to select using class you put a .
and for the name you put nothing
that's just to tell css which one you want to use, you don't want him to chose randomly do you?.


## There are a ton of things in css alone:
we wont cover them in this course, because this course's aim is to get you up and running
search, read the docs and even watch youtube tutorials. 
these stuff are a bit forgetable, if you haven't stummbled uppon a problem, it wont stick with you, and it will be a waste of your time,




 i want to describe how a block would look like
ex:
- have a background color of pink
- cursor become pointer when mouse hover over it
- have a border of 2cm
- have a border color of yellow

it will look like this
```
mydiv{

}
```