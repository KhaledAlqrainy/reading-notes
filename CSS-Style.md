![CSS](https://i.morioh.com/6a6d43417b.png)

# CSS
* We learned before about HTML and how it work but as we saw there is no option for text style or color the text or any modifed that will make our page look good, here comes CSS to make our websites look in a better way.
#### what is CSS?

> Its shortcut for Cascading Style Sheets, which allows us to style our html code and presented to usere.

## How to use?

* in CSS language formula we dont use tags like html only the selctor and then open curly bracket inside it there is a **property** and **vlaue**.


### There is three ways to add css codes:

1- **Inline style** : we write it in each element, ex :
 <h1 style="color:red;">Khaled</h1>


2- **Internal style**  ex :
 <style>
body {
  background-color: Beige;
}

h1 {
  color: blue;
}
</style>

3- **External style** : "Best Practice" 
we write css codes and edits in aonther file than the index html file and we mention a formula in index to let html take css style
 ex :
<head>
<link rel="stylesheet" href="mystyle.css">
<style>
h1 {
  color: Purple;
}
</style></head>


### CSS properties:
* we have many of css properties that can help us make our website look good, Color, we can find it here [CSS properties](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference#index)

### Selectors :
The first thing we do to modifed html in css language is to write which part or code I want to edit it and we call it selector, ex : 
<style>
h1 {
  color: orange;
}
</style>

h1 is a selector.
