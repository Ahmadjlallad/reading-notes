# HTML AND JS

## Starting with HTML

* Structure using semantic elements
  * Example:
  * ```<html>```  tag would represent the start of the code ```<head>``` contain meat data, page title or information about the page all go in ```<head>``` tag, in bellow example ```<head>``` tags have some ```<meta>``` tags inform the browsers about languages, viewport and many more
  * Tags can take attributes like ```<label for="username">User Name</label>``` ```for="username"```  is attribute that tell ```<label>``` about for whom the label.

```#!HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <from > 
    <label for="username">User Name</label>
    <form>
</body>
</html>
```

* Extra Markup
  * ```<!-- comment goes here -->``` write comment in HTML or press "Ctrl+/" for conveniant.

  * id attribute ```<p id="first-p">``` lets the user make a unique identifier for every element, specify one unique id with no repeated id across multiple tags, use mainly for js.

  * Class attribute ```<p class="first-p">``` function like id but, give multipe elementes same class name use manly for CSS.

  * block elements ```<div>```, ```<p>```, ```<ul>``` tags like those counts as block always appear to start on a new line, takes all width space.

  * inline elements ```<span>```, ```<strong>```, ```<img>``` don't take all width don't respict hight.

  * iframe

```#!HTML
<iframe width="704" height="396" src="https://www.youtube.com/embed/Gcos-VJLfPU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

* Grouping
  * ```<div>``` used to make a container, example

``` #!HTML
<div id="header">
<img src="images/logo.gif" alt="Anish Kapoor" />
    <ul>
        <li><a href="index.html">Home</a></li>
        <li><a href="biography.html">Biography</a></li>
        <li><a href="works.html">Works</a></li>
        <li><a href="contact.html">Contact</a></li>
    </ul>
</div><!-- end of header -->
```

* Information about page```<meta>``` It is not visible to users but fulfills several purposes such as telling search engines about your page

```#!HTML

<!DOCTYPE html>
<html>
<head>
<title>Information About Your Pages</title>
<meta name="description"
content="HTML AND JS MARKDOWN" />
<meta name="keywords"
content="HTML, JS, programing languages" />
<meta name="robots"
content="nofollow" />
<meta http-equiv="author"
content="Jon Duckett" />
<meta http-equiv="pragma"
content="no-cache" />
<meta http-equiv="expires"
content="sun, 20 jun 2021 07:59:59 UTC+03:00" />
</head>
<body>
</body>
</html>

 ```

* meta
  * ```<meta name="description" content="This ultimate guide cover all the important aspects of blogging. Find out how to set up a successful blog or to make yours even better!"/>``` meta description attribute describes and summarizes the contents of your page for the benefit of users and search engines.
    ![Exampple](https://yoast.com/app/uploads/2021/03/yoast-seo-meta-description-snippet-3-768x147.png)

  * ```<meta name="keywords"content="HTML, JS, programing languages"/>``` help tell search engines what the topic of the page is.

  * ```<meta name="robots" content="nofollow" />```provide crawlers instructions for how to crawl or index web page content, Not all pages of your website need to be indexed by the search engines. That is why Yoast gives you the possibility to  decide which pages can or can’t be indexed.

  * The ```http-equiv``` attribute provides an HTTP header for the information/value of the ```content``` attribute and The can be used to simulate an HTTP response header.
    * author: This defines the author of the web page.
    * pragma: This prevents the browser from caching the page.
    * expires: Because browsers often cache the content of a page, the expires option can be used to indicate when the page should expire (and no longer be cached). Note that the date must be specified in the format shown.
    * Refresh: Refresh document.

  * Escape Characters: markup sensitive in certain contexts to write <> in HTML without confuse html editor use Escape Characters some example```&lt; => (>), &amp => (&), &quot; => (")```.

* HTML 5 Layout: in HTML 5 divs add a new semantce elemante to replace ```<div>``` .
  * Exampes ```<header>```, ```<nav>```, ```<article>```, ```<footer>```,```<section>```, ```<aside>```,
    * ```<hgroup>``` useed to make sub heading and ```<figure> <figcaption>``` make figure and but caption.
    * Linking around BLock-LeveL elements ```<a>``` element around a block level element that contains child elements. This allows you to turn an entire block into a link.

    ```#!html
    <a href="introduction.html">
    <article>
    <figure>
    <img src="images/bok-choi.jpg"
    alt="Bok Choi" />
    <figcaption>Bok Choi</figcaption>
    </figure>
    <hgroup>
    <h2>Japanese Vegetarian</h2>
    <h3>Five week course in London</h3>
    </hgroup>
    <p>A five week introduction to traditional
    Japanese vegetarian meals, teaching you a
    selection of rice and noodle dishes.</p>
    </article>
    </a>
    ```

* Helping Older Browsers Understand new semantic
  * include which new elements should be rendered as block-level elements

    ```#!CSS
    header, section, footer, aside, nav, article, figure
    {
    display: block;
    ```

  ```#!HTML
  <!--[if lt IE 9]>

  <script src="http://html5shiv.googlecode.com/svn/
  trunk/html5.js"></script>
  <![endif]-->

* Process & Design
  * Know your audience, some example individuals.
    * What is the age range of your target audience?
    * How many hours do they work per week?
    * How often do they use the web?
  * Why People visit the website.
    * visitors goals
  * site maps: organize the information into sections or pages.
  * WireFrames: a simple sketch of the key information that needs to go on each page of a site.

# Java script part

* JS Allows you to make web pages more interactive.(examples)
  * SLIDESHOWS.
  * FORMS.
  * RELOAD PART OF PAGE.
  * FILTERING DATA.

* JS ABC
  * A What is a script & how do I create one?
  * B How do computers fit in with the world around them?
  * C How do I write a script for a web page?

#### A What is a script & how do I create one?

* A script is a series of instructions that a computer can follow to achieve a goal
  * DEFINE THE GOAL.
  * DESIGN THE SCRIPT.
  * CODE EACH STEP.
  * "think" like a computer.

#### B How do computers fit in with the world around them?

* COMPUTERS CREATE MODELS OF THE WORLD USING DATA
  * OBJECTS (THINGS)In computer programming, each physical thing in the world can be represented as an object
    * Each object can have its own:
    * Properties
    * Events
    * Methods
  * PROPERTIES (CHARACTERISTICS) properties of an object, property has a name and a value.

  * EVENTS programs are designed to do different things when users interact with the computer in different ways, script will state which events the programmer wants to respond to, and what part of the script should be run when each of those events occur.

  * Methods represent things people need to do with objects. They can retrieve or update the values of an object's properties
    * Tell you something about that object (using information stored in its properties).
  * Change the value of one or more of that object's properties.
  WEB BROWSERS ARE PROGRAMS BUILT USING OBJECTS

#### C How do I write a script for a web page?

* It is best to keep JavaScript code in its own JavaScript file. 
* The HTML ```<script>``` element is used in HTML pages to tell the browser to load the JavaScript file (rather like the ```<link>``` element can be used to load a CSS file).


