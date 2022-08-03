# 04 - Structure web pages with HTML

## The Definitive Guide on How to Make Your Framework

### An intro to wireframing

1. What is a Wireframe?

    - allows UX designers to plan the info of their design for a website app or product; focuses on how the user processes info on a site

    - plan out where all the info is going before coding

    - a way to know a user interacts with the interface

    - allows you to plan the layout on the of the interface

2. Wireframe examples

    - some draw by hand while others use software like Invision or Balsamiq

    - Wireframes drawn with paper and a pencil, or at a whiteboard, have the advantage of looking and being very easy to change

    - With the help of paper-prototypes, you can test with end users at every stage of ideation and design. Changes at these stages are much easier—and therefore cheaper—than changes deemed necessary after coding is under way.

    - Switching later to software (after initially hand-drawing your wireframe) allows you to keep track of more detailed decisions

3. Things to consider before you start wireframing

    - decision on how to wire frame depends on the situation whether it's about visual design or uncertaintty on what's be designed

    - different design structure:
    Wireframe > Interactive Prototype > Visual > Design
    Sketch > Code
    Sketch > Wireframe > Hi-Def Wireframe > Visual > Code
    Sketch > Wireframe > Visual > Code

4. The best Tools for wireframing

    - UXPin

    - InVision

    _ Wireframe.cc

### 6 Steps to make a Wireframe

1. Do your research

    -carry out analysis of similar product lines

    - be creative

2. Prepare your research for quick reference

    -scribbling a cheatsheet with your business and user goals (your requirements), your personas, use cases, and perhaps some reminders of the coolest features you stumbled across in your competitor research.

3. Make sure you have your user flow mapped out

    - water tight concepts of where users will be coming from

    - good info architecture will make sure users a self sufficient

4. Draft, don’t draw. Sketch, don’t illustrate

    - focus on a rough draft

    - ask yourself these questions along the way:
    How can you organise the content to support your users’ goals?
    Which information should be most prominent? Where should your main message go? What should the user see first when arriving at the page?
    What will the user expect to see on certain areas of the page?
    Which buttons or touch points does the user need to complete the desired actions?

5. Add some detail and get testing

    - add from top to bottom

    - wireframe is skeleton don't add muscle yet // these are ligaments and tendons // usability, simple wording, trust building elements, tooltips for functionality

    - you're ready for user tests at this stage

6. Start turning your wireframes

    - develop prototypes using InVision

### 3 Key Principles

1. Clarity

2. Confidence

3. Simplicity

## HTML Basics

**HyperText Markup Laguage**; foundation that CSS & JavaScript build off of

### So What is HTML

- defines the structure of your content

- consits of elements which you can use to enclose diff parts of the contact to make it act or appear in a certain manner
    ex: My cat is very grumpy  
    If we wanted the line to stand by itself, we could specify that it is a paragraph by enclosing it in paragraph tags:
    <p>My cat is very grumpy</p>

### Anatomy od an HTML element

<p>My cat is very grumpy</p>

- **opening tag**: <p> (name of the element)
    wrapped in opening and closing angle brackets
    states where the element begins or starts to take effect — in this case where the paragraph begins.

- **content**: my cat is very grumpy
    in this case, is just text.

- **closing tag**: </p> (same as opening except with a forward slash before the element name)
    states where the element ends

- **element**: <p>My cat is very grumpy</p>
    opening tag, the closing tag, and the content together comprise the element
    can aslo contain an **attribute**

- **attribute** <p> class="editor-note">My cat is very grumpy </p>
    the attribute contains extra info about the element
    _class_ is the attribute name
    _editor-note_ is the value
    attributes should always have:
        space between it and the element name or previous attribute, if the element already has one or more attributes
        attribute name followed by an equal sign
        attribute value wrapped by opening and closing quotation marks

### Nesting Elements

- **nesting**: elements inside other elements
    <p>My cat is <strong>very</strong> grumpy.</p>
    If we wanted to state that our cat is very grumpy, we could wrap the word "very" in a <strong> element, which means that the word is to be strongly emphasized

- **empty elements**: Some elements have no content

    <img src="images/firefox-icon.png" alt="My test image"> ;contains two attributes, but there is no closing </img> tag and no inner content. This is because an image element doesn't wrap content to affect it. Its purpose is to embed an image in the HTML page in the place it appears

### Anatomy of an HTML document

- <!DOCTYPE html> — doctype.
- <html></html> — the <html> element
- <head></head> — the <head> element

-<meta charset="utf-8"> — can now handle any textual conten

- <title></title> — the <title> element
- <body></body> — the <body>

### Images

<img> <img src="images/firefox-icon.png" alt="My test image">
  embed an image

- src: contains the path to our image

-alt: you specify descriptive text for users who cannot see the image

### Marking up text

- **Headings**

    <h1>-<h6>

- **Paragraphs**

    <p>: <p>This is a single paragraph</p>

-**Lists**: two types of lists unordered (<ul>) and ordered (<ol>)

    each item inside the lists is put inside an <li>
<ul>
  <li>technologists</li>
  <li>thinkers</li>
  <li>builders</li>
</ul>

- **Links**: to add a link <a>; it means anchor

    "Mozilla Manifesto"
    Wrap the text in an <a> element, as shown below:
    <a>Mozilla Manifesto</a>
    Copy to Clipboard
    Give the <a> element an href attribute, as shown below:
    <a href="">Mozilla Manifesto</a>
    Copy to Clipboard
    Fill in the value of this attribute with the web address that you want the link to

## Semantics

### Semantics in HTML

- **Benefits**: 
    Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
    Screen readers can use it as a signpost to help visually impaired users navigate a page
    Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
    Suggests to the developer the type of data that will be populated
    Semantic naming mirrors proper custom element/component naming

