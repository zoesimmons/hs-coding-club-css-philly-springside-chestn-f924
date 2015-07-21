# What Not To Wear - CSS Edition
## You won't believe these changes!

###The "Befores"

**Buzzfeed**

<img src="https://s3.amazonaws.com/after-school-assets/buzzfeed-before.png">

**New York Times**

<img src="https://s3.amazonaws.com/after-school-assets/new-york-times-before.png">

**Beyonce.com**
<img src="https://s3.amazonaws.com/after-school-assets/beyonce-before.png">


**Pretty rough huh?**  These guys clearly do not know how to dress for their size, style, and accessories? Non-existent. In fact, there is literally no stylin involved in either website. This is what Buzzfeed, The New York Times, and Beyonce look with just plain and simple text. How in the world are Stacy London and Clinton Kelly going to makeover these three websites in an hour TV segment? They have their work cut out for them.
 

###The "Afters"

**Buzzfeed**

<img src="https://s3.amazonaws.com/after-school-assets/buzzfeed-after.png">

**New York Times**

<img src="https://s3.amazonaws.com/after-school-assets/nytimes-after.png">

**Beyonce.com**

<img src="https://s3.amazonaws.com/after-school-assets/beyonce-after.png">


###Let's Get Started

How in the world did they make those changes so quickly? The difference between the "Before" and "After" are pretty drastic. All three companies used CSS to add styling and a specific layout to their page. CSS, Cascading StyleSheet, is a programming language that makes up the beauty of the web we see today. Without it, we would be looking at black text on a white screen. 

####Step 1:

Before we can add styling, we need to have an HTML file. We've provided you with `beyonce.html`. This file contains just the raw content of beyonce.com. We'll be making changes to this file to upgrade the look and feel. Because we're the style-gurus and Beyonce needs our help.

To look at this file in the browser, like you would a normal website, in the Nitrous terminal in the directory for this project, enter `python -m SimpleHTTPServer 3000`. Once you have the server running, select `preview` and then `port 3000`.

<img src="https://s3.amazonaws.com/after-school-assets/nitrous-preview.png" alt="nitrous preview">

From there, you'll want to select the `beyonce.html` file:

<img src="https://s3.amazonaws.com/after-school-assets/open-beyonce-html-nitrous.png" height="200px">

####Step 2: 

We always write our CSS in a different file. In programming, we like to separate different tasks to different files. This is known as separation of concerns. What this means is that we have one file to write our HTML and at least one different file to write our CSS.

The developers of beyonce.com happened to write the CSS and store it online so we can take a look.

<a href="http://www.beyonce.com/wp-content/plugins/search-everything/static/css/se-styles.css?ver=4.2.1">StyleSheet 1</a>

<a href="http://www.beyonce.com/wp-content/themes/beyonce_2014/assets/stylesheets/styles.css?ver=4.2.1">StyleSheet 2</a>

#### Step 3:

Now that we have our HTML file and our CSS files, we need to link them. Essentially, our `beyonce.html` file needs to know to load both of the CSS files to apply styling.

Inside of our HTML, we need to add two `link` tags. Copy the link tags below and paste them in `beyonce.html` where you see the comment `<!-- CSS LINK GOES HERE -->`.

```html
  <link rel='stylesheet' id='se-link-styles-css'  href='http://www.beyonce.com/wp-content/plugins/search-everything/static/css/se-styles.css?ver=4.2.1' type='text/css' media='all' />
  <link rel='stylesheet' id='app-css-css'  href='http://www.beyonce.com/wp-content/themes/beyonce_2014/assets/stylesheets/styles.css?ver=4.2.1' type='text/css' media='all' />
```
Once you've saved your changes, reload the page you opened in the browser to see the styling added!

### Tell Me More About The Code

Now that we're familiar with what CSS is, the role that it plays in a website, and how to link it to our HTML, let's learn how to write our own CSS.

Again, we need our own HTML file. You can find a basic HTML file located in `index.html`

  



