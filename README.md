# What Not To Wear - CSS Edition
## You won't believe these changes!

###The "Befores"

**Buzzfeed**

<img src="https://s3.amazonaws.com/after-school-assets/buzzfeed-before.png">

**New York Times**

<img src="https://s3.amazonaws.com/after-school-assets/new-york-times-before.png">

**Beyoncé.com**

<img src="https://s3.amazonaws.com/after-school-assets/beyonce-before.png">


**Pretty rough huh?**  These guys clearly do not know how to dress for their size, style, and accessories? Non-existent. In fact, there is literally no styling involved in any of the websites. This is what Buzzfeed, The New York Times, and Beyoncé look with just plain and simple text. How in the world are Stacy London and Clinton Kelly going to makeover these three websites in an hour TV segment? They have their work cut out for them.
 

###The "Afters"

**Buzzfeed**

<img src="https://s3.amazonaws.com/after-school-assets/buzzfeed-after.png">

**New York Times**

<img src="https://s3.amazonaws.com/after-school-assets/nytimes-after.png">

**Beyoncé.com**

<img src="https://s3.amazonaws.com/after-school-assets/beyonce-after.png">


###Let's Get Started

Woah Stacy and Clinton work fast! They made those changes so quickly! The differences between the "Before" and "After" are all pretty drastic. All three companies used CSS to add styling and a specific layout to their page. CSS, which stands for Cascading Style Sheet, is a programming language that makes the beauty of the web we see today. Without it, we would only be looking at "Before" versions of every single website.

####Step 1:

Before we can add styling, we need to have an HTML file. We've provided you with `Beyonce.html`. This file contains just the raw content of Beyonce.com. We'll be making changes to this file to upgrade the look and feel, because we're the style-gurus and Beyoncé needs our help.

In order to access this lesson and edit files, please click the `Open in Nitrous` button at the top of the page.

<img src="https://s3.amazonaws.com/after-school-assets/open-in-nitrous.png">

####Step 2:

To view `Beyonce.html` in the browser, like you would a normal website, in the Nitrous terminal in the directory for this project, enter `python -m SimpleHTTPServer 3000`. 

Once you have the server running, select `preview` and then `port 3000`.

<img src="https://s3.amazonaws.com/after-school-assets/nitrous-preview.png" alt="nitrous preview">

From the browser you just opened (should be a super simple mostly white page with a couple links), select the `beyonce.html` file.

<img src="https://s3.amazonaws.com/after-school-assets/open-beyonce-html-nitrous.png" height="200px">

Take a look at `beyonce.html` in the Nitrous text editor too. Notice how the developers that built her site put their logo in huge block letters at the top? Comments never show up in the actual website, and are a great way to leave notes from developers to other developers. [Top Tip: You can create comments in HTML by surround your comment with `<!-- -->`.


####Step 3: 

We always write our CSS in a different file. In programming, we like to separate different tasks to different files. This is known as separation of concerns, which means we have one file to write our HTML and at least one different file to write our CSS.

The developers of Beyonce.com happened to write the CSS and store it online so we can take a look. Don't worry if the code looks really overwhelming and confusing. The code is all smooshed together and is hard to decipher, but pieces of the code will start to make sense by the end of this lesson!

Take a look now for funsies--the next step is about linking these two style sheets to our HTML file, `beyonce.html` so we can make the raw content beautiful.

<a href="http://www.beyonce.com/wp-content/plugins/search-everything/static/css/se-styles.css?ver=4.2.1">StyleSheet 1</a>

<a href="http://www.beyonce.com/wp-content/themes/beyonce_2014/assets/stylesheets/styles.css?ver=4.2.1">StyleSheet 2</a>

#### Step 4:

Now that we have our HTML file and our CSS files, we need to link them. Essentially, our `beyonce.html` file needs to know to load both of the CSS files to apply styling.

Inside of our HTML, we need to add two `link` tags. Copy the link tags below and paste them in `beyonce.html` where you see the comment `<!-- CSS LINK GOES HERE -->`. You can use a typical browser screen search to find that particular portion of the code.

```html
  <link rel='stylesheet' id='se-link-styles-css'  href='http://www.beyonce.com/wp-content/plugins/search-everything/static/css/se-styles.css?ver=4.2.1' type='text/css' media='all' />
  <link rel='stylesheet' id='app-css-css'  href='http://www.beyonce.com/wp-content/themes/beyonce_2014/assets/stylesheets/styles.css?ver=4.2.1' type='text/css' media='all' />
```
Once you've saved your changes, refresh the page you opened in the browser to see the styling added!

#### Step 5:

It's time to store your work on Github and mark this lesson as complete on Learn (you can keep reading on to learn more about writing your own CSS!).

In terminal, in Nitrous, enter `learn submit`. Voila!

#### Step 6: Share Share Share!

You just helped Beyoncé! Talk about a cool moment. Screenshot the fixed site or the code and share with **\#flatironcodeclub** and **\#styledbeyonce**

### Tell Me More About The Code

Now that we're familiar with what CSS is, the role that it plays in a website, and how to link it to our HTML, let's learn how to write our own CSS.

Again, we need our own HTML file. You can find a basic HTML file, `index.html` located in a directory called `your-css`.

Before you can do anything else, you need to shut down the server that is loading `Beyoncé.html` for us. You can do that by hitting `control` + `c`.

Now, you'll want to move into the `your_css` directory by entering in terminal: `cd your_css`.

`cd` is a command that stands for "change directory". This moves our location from one directory to another.

#### Linking CSS
The first thing we need to do is link our CSS file to our HTML file. Copy and paste the `link` tag below in between the opening and closing `<head>` tag in `index.html` (either above or below the `<title>` tag is fine):

```html
<head>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
```

Don't forget to save your changes after you edit your file!

The link tag has three attributes `rel`, `type`, and `href`. 

`rel` is the relationship of the type of file we're linking to our HTML. In this case, it's a style sheet.

`type` is the type of file we're linking. Here it's a text/css file.

`href` is the hyper-reference to the file we're linking. The `style.css` file is located in the same directory as `index.html` so we just have to link the file name.

So far, we've just linked our CSS file to our HTML file. Websites typically will have several CSS files (Beyoncé has two), as well as several JavaScript files that handle all the animations on a website. Don't worry too much about JavaScript right now, we'll get into that in the next Unit.

It's important to note here that HTML and CSS are different languages, written in different files that have authority over different roles of our website. As we can see from the Befores and Afters, CSS plays an incredibly important role in displaying the content of our websites in visually appealing ways. The rest of the lessons in this unit will walk you through how to make stunning websites, just like the developers for beyonce.com.

#### Opening Our Code In The Browser

In terminal inside the `your-css` directory, enter `python -m SimpleHTTPServer 3000`. This will start a sever so we can view our code.

Then select `Preview` and `port 3000` just like we did to view `Beyoncé.html`:

<img src="https://s3.amazonaws.com/after-school-assets/nitrous-preview.png" alt="nitrous preview">

This time, our `index.html` file will automatically load in the browser.

Make sure to shut down your server by hitting `control` and `c` so you can keep working on the rest of the lesson!

You'll notice in the `head` tag, there no CSS file has been linked. The first step, before we can write any CSS is to link our HTML file. Copy and paste the code below inside your `head` tag (either above or below the `title` tag):

```html
<link rel="stylesheet" href="style.css">
```

Make sure you save your changes!

#### Writing CSS

Next, you'll want to use the file navigator in Nitrous to open `style.css` in the text editor. You'll be coding your solutions there. 

Let's say we want to add specific styling to the text inside our `h1` tag. We want to make the text color red and the font size 200px.

Inside of our `style.css` file we'd write:

```css
h1 {
  color: red;
  font-size: 200px;
}
```

We tell CSS that we're adding specific styling to our `h1` tag. This is called the CSS selector. We're selecting what text we want to add styling to by typing the name of the HTML tag. We assign the specific styling inside the `{}`.

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
<p id="paragraph-one"> Bacon ipsum dolor amet venison turducken sirloin filet mignon. Shoulder porchetta kevin beef turducken corned beef. Fatback short loin beef, venison drumstick cow chuck corned beef. Shoulder t-bone swine rump pancetta ribeye, picanha spare ribs boudin hamburger biltong chicken pig drumstick turducken. Meatball doner shank boudin ham brisket. Jerky meatball pancetta shoulder, pork kevin swine. Biltong drumstick shankle, cupim sausage tenderloin pastrami shank flank.</p>
```
An ID is an attribute of an HTML tag that acts as a specific and unique identifier for that particular piece of content. You cannot repeat IDs in a website. 

Inside our CSS, we need to select the text inside the tag with the ID paragraph-one, instead of just p. Delete the original paragraph styling we wrote and replace it with this styling for just the text that we gave the unique ID to. 

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





  



