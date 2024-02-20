# Change Style

**Changing the assigned style by clicking on a designated area on the screen with JS and CSS.**

You can replace an assigned style with another assigned style.

To do this, you should start by using the JS function below.

## JS 

      function changeStyle() {
      var element = document.body;
        element.classList.toggle("change");
      }

When we run the changeStyle function, it toggles to the class we prepared in the CSS file.

You can see example CSS styles below.

## CSS

      body {
        background: #121212;
        color: #F5F5F5;
        text-align: center;
      }

      .change {
        background: #F5F5F5;
        color: #121212;
        text-align: left;
      }

Then I defined a class called .change.

Here I defined a different background, color, text-align.

When my JS function was run, it triggered the styles inside the .change class and the site design changed.

You can also see sample HTML codes below.

## HTML

    <html>
      <head>
        <meta charset="UTF-8">
        <title>Change Style</title>
        <link rel="stylesheet" type="text/css" href="css/changeStyle.css"/>
      </head>
      <body>
        <h1 onclick="changeStyle()">Click to change styles</h1>
        <script src="js/changeStyle.js"></script>  
      </body>
    </html>


I ran my JS function with onclick="changeStyle()".

For example, I ran it with the h1 tag.

You can run it with anywhere you want.
