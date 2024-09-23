## Day 1 

## Javascript Can Be Added To a Webpage in the following Ways 
* Inline Script 
* Internal Script
* External Script 
* Multiple External Scripts

Inline Script 
Rather than importing a external javascript file, some scripts can be directly embedded inside the HTML file. These are called inline scripts and can be directly embedded into an html element via an event attribute. 

```
<div onclick="alert('HELLO')"></div>
```

External Scripts

External Scripts can be added into the Header or the Body of an HTML document. This is done by adding a script HTML tag with the src property pointing to the location of the file. 


Script In Head
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>This is an HTML Document</title>
        <script src="intro.js"></script>
    </head>
    <body></body>
</html>
```

Script In Body
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>This is an HTML Document</title>
    </head>
    <body>
      <script src="intro.js"></script>
    </body>
</html>
```

Multiple External Scripts

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>This is an HTML Document</title>
    </head>
    <body>
      <script src="intro.js"></script>
      <script src="main.js"></script>
    </body>
</html>
```

Your main.js file should be below all other scripts. It is very important to remember this.

