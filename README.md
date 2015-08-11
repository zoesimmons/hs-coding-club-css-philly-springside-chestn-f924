# What Not To Wear - CSS Edition
## You won't believe these changes!

###The "Befores"

**Buzzfeed**

<img src="https://s3.amazonaws.com/after-school-assets/buzzfeed-before.png">

**New York Times**

<img src="https://s3.amazonaws.com/after-school-assets/new-york-times-before.png">

**Beyonce.com**

<img src="https://s3.amazonaws.com/after-school-assets/beyonce-before.png">


**Pretty rough huh?**  These guys clearly do not know how to dress for their size, style, and accessories? Non-existent. In fact, there is literally no styling involved in either website. This is what Buzzfeed, The New York Times, and Beyonce look with just plain and simple text. How in the world are Stacy London and Clinton Kelly going to makeover these three websites in an hour TV segment? They have their work cut out for them.
 

###The "Afters"

**Buzzfeed**

<img src="https://s3.amazonaws.com/after-school-assets/buzzfeed-after.png">

**New York Times**

<img src="https://s3.amazonaws.com/after-school-assets/nytimes-after.png">

**Beyonce.com**

<img src="https://s3.amazonaws.com/after-school-assets/beyonce-after.png">


###Let's Get Started

How in the world did they make those changes so quickly? The difference between the "Before" and "After" are all pretty drastic. All three companies used CSS to add styling and a specific layout to their page. CSS, which stands for Cascading StyleSheet, is a programming language that makes the beauty of the web we see today. Without it, we would be looking at black text on a white screen. 

####Step 1:

Before we can add styling, we need to have an HTML file. We've provided you with `beyonce.html`. This file contains just the raw content of beyonce.com. We'll be making changes to this file to upgrade the look and feel, because we're the style-gurus and Beyonce needs our help.

In order to access this file, take a look at the `How To: Work On A Lab` to fork and clone this lesson.

####Step 2:

To view `beyonce.html` in the browser, like you would a normal website, in the Nitrous terminal in the directory for this project, enter `python -m SimpleHTTPServer 3000`. 

Once you have the server running, select `preview` and then `port 3000`.

<img src="https://s3.amazonaws.com/after-school-assets/nitrous-preview.png" alt="nitrous preview">

From there, you'll want to select the `beyonce.html` file:

<img src="https://s3.amazonaws.com/after-school-assets/open-beyonce-html-nitrous.png" height="200px">

####Step 3: 

We always write our CSS in a different file. In programming, we like to separate different tasks to different files. This is known as separation of concerns, which means we have one file to write our HTML and at least one different file to write our CSS.

The developers of beyonce.com happened to write the CSS and store it online so we can take a look. Don't worry if the code looks really overwhelming and confusing. The code is all smooshed together and is hard to decifer. Pieces of the code will start to make sense by the end of this lesson!

<a href="http://www.beyonce.com/wp-content/plugins/search-everything/static/css/se-styles.css?ver=4.2.1">StyleSheet 1</a>

<a href="http://www.beyonce.com/wp-content/themes/beyonce_2014/assets/stylesheets/styles.css?ver=4.2.1">StyleSheet 2</a>

#### Step 4:

Now that we have our HTML file and our CSS files, we need to link them. Essentially, our `beyonce.html` file needs to know to load both of the CSS files to apply styling.

Inside of our HTML, we need to add two `link` tags. Copy the link tags below and paste them in `beyonce.html` where you see the comment `<!-- CSS LINK GOES HERE -->`.

```html
  <link rel='stylesheet' id='se-link-styles-css'  href='http://www.beyonce.com/wp-content/plugins/search-everything/static/css/se-styles.css?ver=4.2.1' type='text/css' media='all' />
  <link rel='stylesheet' id='app-css-css'  href='http://www.beyonce.com/wp-content/themes/beyonce_2014/assets/stylesheets/styles.css?ver=4.2.1' type='text/css' media='all' />
```
Once you've saved your changes, reload the page you opened in the browser to see the styling added!

### Tell Me More About The Code

Now that we're familiar with what CSS is, the role that it plays in a website, and how to link it to our HTML, let's learn how to write our own CSS.

Again, we need our own HTML file. You can find a basic HTML file, `index.html` located in a directory called `your-css`. In terminal, you'll want to move into the `your_css` directory by entering in terminal `cd your_css`. `cd` is a command that stands for change directory. This moves our location from one directory to another.

#### Linking CSS
The first think we need to do is link our CSS file to our HTML file. Copy and paste the `link` tag below inside your `head` tag in `index.html`

```html
<head>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
```

The link tag has three attributes `rel`, `type`, and `href`. 

`rel` is the relationship of the type of file we're linking to our HTML. In this case, it's a stylesheet.

`type` is the type of file we're linking. Here it's a text/css file.

`href` is the hyper-reference to the file we're linking. The `style.css` file is located in the same directory as `index.html` so we just have to link the file name.

#### Opening Our Code In The Broswer

In terminal inside the `your-css` directory, enter `python -m SimpleHTTPServer 3000`. This will start a sever so we can view our code.

Then select `Preview` and `port 3000` just like we did to view `beyonce.html`:

<img src="https://s3.amazonaws.com/after-school-assets/nitrous-preview.png" alt="nitrous preview">

This time, our `index.html` file will automatically load in the browser.


#### Writing CSS

Now, let's say we want to add specific styling to the text inside our `h1` tag. Let's say we want to make the text color red and the font size 200px.

Inside of our `style.css` file we'd write:

```css
h1 {
  color: red;
  font-size: 200px
}
```

We tell CSS that we're adding specific styling to our `h1`. This is called the CSS selector. We're selecting what text we want to add styling to. We assign the specific styling inside the `{}`.

CSS is comprised of a series of properties and values. In this case, were using the `color` and `font-size` properties. After every property, we put a `:` and after every value we put a `;`. It's important to note that our CSS will break if we're not specific with our syntax.

After we save our changes, we can refresh the page in the browser and see the styling changes we made!


#### Changing Just ONE paragraph
Now let's try and change the font-styling of the first paragraph to italics.

```css
p {
  font-style: italic;
}
```
Save your changes and refresh. Notice that it changed not just the first paragraph, but also the second and the third. So how can we add styling to just one?! obviously using `p` as our CSS selector is selecting the text inside _every_ `p` tag on the page.

We can do that by modifying both our HTML and our CSS. 

Inside our HTML, we need to add `id="paragraph-one"` inside our very first opening `p` tag:

```html
<p id="paragraph-one"> Bacon ipsum dolor amet venison turducken sirloin filet mignon. Shoulder porchetta kevin beef turducken corned beef. Fatback short loin beef, venison drumstick cow chuck corned beef. Shoulder t-bone swine rump pancetta ribeye, picanha spare ribs boudin hamburger biltong chicken pig drumstick turducken. Meatball doner shank boudin ham brisket. Jerky meatball pancetta shoulder, pork kevin swine. Biltong drumstick shankle, cupim sausage tenderloin pastrami shank flank.<p>
```
An ID is an attribute of an HTML tag that acts specific and unique identifier for that particular piece of content. You cannot repeat IDs in a website. 

Inside our CSS, we need to select the text inside the tag with the id `paragraph-one`, instead of just `p`.

```css
#paragraph-one {
  font-style: italic;
}
```

In our HTML we defined an ID on the first `p` tag. We then used that ID as our CSS selector, and applied that styling to our text.

Save both `index.html` and `style.css` and refresh in the browser!


#### Adding Styling To More Than One Paragraph

What if we wanted the same styling to the second and the third paragraph? We want the text size to be 25px and the font color to be green. IDs can only be used one time per web site. IDs have to be unique, which means we can't define the same ID to two different paragraph tags.

Instead, we uses classes. A `class` is another HTML tag attribute that identifies a group of tags that want to have the same styling. You can have the same class repeated as many times as you want in your HTML.

Inside your `index.html`, add `class="two-paragraphs"` inside the opening `p` tag of both paragraphs.

```html
<p class="two-paragraphs">Leberkas t-bone kielbasa prosciutto pancetta, drumstick picanha pork belly cow meatball venison spare ribs landjaeger fatback. Pork shank boudin jerky venison. Salami pork chop leberkas beef. Bacon porchetta shoulder, cow strip steak prosciutto chicken beef. Bresaola drumstick flank chuck, frankfurter picanha brisket spare ribs andouille jerky ball tip leberkas.</p>

<p class="two-paragraphs">Short ribs jowl ham hock short loin venison fatback salami drumstick jerky beef ribs filet mignon boudin t-bone swine. Swine biltong tongue, salami beef bacon porchetta tri-tip. Tongue rump spare ribs ball tip salami, chuck sausage corned beef landjaeger cupim frankfurter. Pork belly brisket sirloin alcatra.</p>
```

In our CSS, we can use the class as our CSS selector. Copy and paste the code below inside your `style.css`:

```css
.two-paragraphs {
  font-size: 25px;
  color: green;
}
```

Save both `index.html` and `style.css` and refresh!


### Want To Learn More?

No need to memorize all those CSS properties. Take a look at these great resources.

1 [Mozzilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_started)

2 [Learn Layout](http://learnlayout.com/)

3 [CodeAcademy CSS Glossary](http://www.codecademy.com/glossary/css)

4 [w3schools](http://www.w3schools.com/cssref/)

5 [Colour Lovers](http://www.colourlovers.com/)





  



