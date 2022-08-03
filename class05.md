# Read: 05 - Design web pages with CSS

## What is CSS

Stands for **Cascading Style Sheets**; creates great looking web pages

### What is CSS for

- language for specidfying how docs are presented to users
  - doc is a text file structured using a markup language
        HTML, VG, XML

- PRESENTING a doc means converting it to a usable for the audience

- can be used to create a layout including color or turning a single column of text into a layout with a main content area and a sidebar for related informstion

### CS Syntax

- rule based language

- show main heading as large red text so the code would be : "h1 {
    color: red;
    font-size: 5em;
}" 

- this rule opens with a selector (selects the HTML element that we are going to style); 

- then have a set of curly braces; 

- inside the braces is one or more **declaration** which take the form of **property** or **value** 

- property is color which is before the colon and we specify the value of the prop after the colon which is red

- example contains two declaration one for color and the other for font-size; Each pair specifies a property of the element(s) we are selecting (<h1> in this case), then a value that we'd like to give the property

- CSS properties have diff values dependant on which is being specified // in this case *color* and *font-size*

### CS Modules

-broken down into modules

- many documentation pages are organized around a particular module

- ex: **the Backgrounds and Borders module** — you might think that it makes logical sense for the background-color and border-color properties to be defined in this module.

### CS Specifications

- new features are developed by the CSS working group (W3C)

- imperative to understand the relationship between the CSS you are using and the browser support

### Browser Support Information

- browser support status is shown on ever MDN CSS property page in a place called browser compatibility

- check how the property works

## How to Add CSS

### Three ways to insert CSS

- External

- Internal

- Inline

#### External CSS

- change the look of an entire website by changing one file

- Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section

- external styles are defined by // <link> element, inside the <head> section of an HTML page

- can be written in any text editor but must be saved with a .css extension

- ex: "mystyle.css"
body {
  background-color: lightblue;
}

h1 {
  color: navy;
  margin-left: 20px;
}

#### Internal CSS

- one single HTML page has a unique style

- defined inside the <style> element, inside the <head> section

#### Inline CSS

- used for unique sryle of s ingle element 

- add the style attribute to the relevant element

- defined within the "style" attribute of the relevant element

### Multiple Style Sheets

- if some properties have been defined for the same elements in different style sheets then the **LAST** read style will be used

ex:
external has h1 {color: navy;}
internal has h1 {color: orange;}
the color will be orange

### Cascading Order

- What style will be used when there is more than one style specified for an HTML element?

- styles in a page will "cascade" into a new "virtual" style sheet by the following rules, where number one has the highest priority:

Inline style (inside an HTML element)
External and internal style sheets (in the head section)
Browser default
So, an inline style has the highest priority, and will override external and internal styles and browser defaults.

## CSS Color Property

- color property specifies the color of text

    - set it w a **Hex value** // body {color: #92a8d1;}

    - **RGB value** // body {color: rgb(201, 76, 76);}

    - **RGBA value** // body {color: rgba(201, 76, 76, 0.6);}

    - **HSL value** // body {color: hsl(89, 43%, 51%);}

    - **HSLA value** // body {color: hsla(89, 43%, 51%, 0.6);}