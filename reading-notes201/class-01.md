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
