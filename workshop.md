# jQuery + Bootstrap == <3

A Match Made in Open Source Heaven

## Hi, I'm Alan

 * 8 Years of development experience
 * I've taught for Girl Develop It, Grand Circus, Apigee
 * I started Apprend
 * Freelance as 13protons -  Web Dev & Graphic Design

## Here's how you can contact me

 * @apprenddetroit
 * alan@apprend.org
 * (734) 707-1908

 Please tweet responsibly

# Apprend

<img src="http://apprend.org/images/apprend-logo.png" class="logo" alt="Apprend Logo
"/>

Apprend is a new tech education company in Detroit. We're building curriculum and holding classes throughout 2015.

---

This presentation is a test run for a longer-form jQuery + Bootstrap class that's coming up March 23.

## Join Apprend's Mailing List

Please join our monthy-ish mailing list to find out about all the great events that are being scheduled. You can find it by visiting [apprend.org](/) and scrolling to the bottom of the home page.

![Mailing List SS](http://apprend.github.io/jquery-bootsrap-workshop/images/mailing-list-ss.png)

## Get Involved

If you want to get involved with Apprend as a student or instructor, please join our meetup group at [meetup.com/apprend](http://meetup.com/apprend).

![Apprend Meetup](http://localhost:3000/images/apprend_meetup.png)

## Upcoming Events

[**Intro to Programming**](http://apprend.org/events/2015/February-Into-To-Programming/)
Learn how to program in JavaScript over 4 nights.
Monday March 2 - Wednesday March 11, $180

[**jQuery + Bootsrtap**](http://apprend.org/events/2015/jQuery-Bootstrap/)
Two day, 6 hour, class for creating more dynamic and sophisticated web sites.
Monday March 23 - Wednesday March 25, $75

# Goals for today

  * Learn why Bootsrap + jQuery are such a big deal
  * Cover Bootstrap's basics
  * Create a *somewhat* historically accurate page named "A Tale of Two Hotdogs"

# What is Bootstrap?

---

![B Logo](https://www.leyder-consulting.com/images/bootstrap.png)

*"Bootstrap is the most popular HTML, CSS, and JS framework for developing responsive, mobile first projects on the web"*

> Bootstrap was created by a handful of engineers at Twitter in 2010, and released as an open source project in August of 2011.

[Some Stats](https://github.com/twbs/bootstrap), [Kitchen Sink Example](http://getbootstrap.com/examples/theme/)

# What is jQuery?

---

![jQUery Logo](http://roblaplaca.com/blog/wp-content/uploads/2013/12/jquery-logo-520x245.jpg)

*"jQuery is a fast, small, and feature-rich JavaScript library. It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers."*"

> jQuery was created by John Resig is 2005 as a way to bring a degree of simplicity to what he saw as a messy and hard to learn interface between webpages and JavaScript.


# Why they == <3

Bootstrap is built on jQuery, and both tools were designed to dramatically up **your** productivity.

---

Both jQuery and Bootstrap save you from having to understand the minute differences between modern web browsers, and allow you to focus on building your website.

## A Bit of Perspective

Bootstrap and jQuery allow the average person a huge leap in productivity when building a web page, and are both incredibly useful and well loved bits of software.

They do not, however, save you from needing to understand the fundamentals of the HTML, CSS, and JavaScript they are built from.

# Bootstrap Basics

## Bootstrap is a Library

Bootstrap is a library, and you need to include it in your page for it to work. Try their CDN hosted stylesheet and JavaScript files.

```html
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">

<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js"></script>
```

## jQuery Required

All of Bootstrap's JavaScript plugins require jQuery to be included - so don't forget it

```html
<script src="//code.jquery.com/jquery-1.11.2.min.js"></script>
```

## Using the Tools

There are 3 major way that you can pull Bootstrap into your project:

Component   |  How
------------|----------
CSS         |  Add classes to your existing markup
Components  |  Copy/Paste HTML snippets + modify them
JavaScript  |  Copy/Paste HTML & JS Snippets + modify them

## CSS

Bootstrap's CSS is expansive - the raw stylesheet is over 6000 lines long! Think of that as 6000 lies you don't have to write. In it you get tons of goodies:

* A 12 column mobile-first grid system
* Thoughtful default typographic styles, based on [normalize](http://necolas.github.io/normalize.css/)
* Pretty Tables
* Useful default forms
* A unified button system
* Responsive images
* Semantic Helper classes
* + Lots more

## Components

Bootstrap's Components are probably what you all came for. They are an expansive list of common UI patterns that you can just copy/paste into your project.

Components include: **Glyphicons, Dropdowns, Button groups, Button dropdowns, Input groups, Navs, Navbar, Breadcrumbs, Pagination, Labels, Badges, Jumbotron, Page header, Thumbnails, Alerts, Progress bars, Media object, Default media, Media list, List group, Panels, Responsive embed, Wells**

[Demo](http://www.bootply.com/render/65566)

## JavaScript

Bootstrap's JavaScript plugins go above and beyond with things like dropdown menus, tooltips, buttons with loading state, and modal windows.

All of these plugins are written as jQuery plugins, and are incredibly flexible. You can generally hook into events at every stage of a plugin's useage in the UI, such as on load, click, event end, destroy, etc.

[Demo](http://getbootstrap.com/javascript/)

## Themes

![Saywhat?](http://apprend.github.io/jquery-bootsrap-workshop/images/saywhat.jpg)

Bootstrap can be themed. Just google it.

[The Wall](http://getbootstrap.com/customize/)

## Recap - What just happened?

Bootstrap has three ways of accessing it's tools - CSS, Components, and JavaScript plugins.

Bootstrap can be themed, saving you even more work.

## Questions?

Do you have any questions before we start writing some code?

# A Tale of Two Hotdogs

### What are we going to build?

We're going to put together a single-page website that uses these components:

 * Based on the bootstrap 'cover' template
 * A bootstrap button
 * A modal dialog
 * A bootstrap circular image
 * A custom glyphicon

---

![A Tale of Two Hotdogs](http://apprend.github.io/jquery-bootsrap-workshop/images/a-tale-of-two-hotdogs.jpg)

It should look something [like this](http://apprend.github.io/jquery-bootsrap-workshop/) when we're done.


## Step 0: Don't follow along yet

Normally, you'd download Bootstrap from [getbootstrap.com/](http://getbootstrap.com/), optionally download an example layout, and hack around with it a bit before getting to building YOUR page.

You DON'T have to download Bootstrap, just get the template pre-built for this exercise...

## Download The Template

Head over to this url and click on the "Download Zip" button in the lower right corner of the page:

[github.com/apprend/jquery-bootsrap-workshop](https://github.com/apprend/jquery-bootsrap-workshop)

![download](http://apprend.github.io/jquery-bootsrap-workshop/images/download.png)

## Bootstrap is already installed

If you open up `index.html` you should see the Bootstrap css & js files already included:

```html
    <title>Cover Template for Bootstrap</title>

    <!-- Latest compiled and minified CSS -->
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">
    ...


```

## Before we get crackin'

Remember that you need to save your html file and reload the page in your browser to see changes.

> One more time

You need to save your html file and reload the page in your browser to see changes.

### Background Image

Modifying the background image has nothing to do with Bootstrap *per-se*, but we're hacking on the pre-bulit bootstrap template.

Add this to `css/apprend.css`

```css
body {
  background-image: url('../images/12nGriswold_1920.jpg');
  background-size: cover;
}
```

###  Customize Main Text & Title

Now let's change the text to relate to the background photo.

Open `index.html`, and edit near line 52:

```html
  <div class="inner cover">
    <h1 class="cover-heading">Cover</h1>
    <p class="lead">
      ...something witty goes here...
    </p>
```

Change "Cover" to "A Tale of Two Hotdogs", and fill the paragraph with text from [apprend.github.io/jquery-bootsrap-workshop/](http://apprend.github.io/jquery-bootsrap-workshop/).

### Modify Page Title

In `index.html`, change

```html
<h1 class="cover-heading">Cover</h1>
```

to read

```html
<h1 class="cover-heading">Detroit History</h1>
```

### Icon in Title

To get an icon in the title, we can use glyphicions.

Drop an icon from the "How to Use" section of the [Bootstrap Components page](http://getbootstrap.com/components/#glyphicons) inside the `h1` we just edited

```html
<h1 class="cover-heading">
  <span class="glyphicon glyphicon-search" aria-hidden="true"></span>
  Detroit History
</h1>
```

> Change 'search' to 'fire', or anything else you want. Cool, huh?


### Cony Pic

First things, first, just drop in a regular ole' image tag right above our `h1` inside our `div.inner.cover`:

```html
<img src="images/coney.jpg" />
```
---

[According to the Bootstrap website](http://getbootstrap.com/css/#images-shapes), we just have to add a class of `img-circle` to get a round image.

```html
<img src="images/coney.jpg" class="img-circle" />
```

> Boom - round coney pic.

# Recap - What Just Happened

So far, we grabbed a stock bootstrap template with the CDN links already added for us, modified some of text, added an icon by changes a class, and created a nice rounded thumbnail image.

### Check In

Let's compare our in-progress site, to our goal: [apprend.github.io/jquery-bootsrap-workshop/](http://apprend.github.io/jquery-bootsrap-workshop/)

### Add the a Modal dialog

Drop in the modal code from [getbootstrap.com](http://getbootstrap.com/javascript/#modals-related-target) into `index.html` before the closing tag for `.site-wrapper`.

```html
<!-- Modal -->
<div class="modal fade" id="myModal" tabindex="-1" role="dialog" aria-labelledby="myModalLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
        <h4 class="modal-title" id="myModalLabel">Detroit History wants to hear from you!</h4>
      </div>
      <div class="modal-body">
        <form>
          <div class="form-group">
            <label for="message-text" class="control-label">Message:</label>
            <textarea class="form-control" id="message-text" placeholder="Give me 2 with everything"></textarea>
          </div>
        </form>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-default" data-dismiss="modal">Cancel</button>
        <button type="button" class="btn btn-primary">Send Message</button>
      </div>
    </div>
  </div>
</div>
```

### Add a button to trigger the Modal

Now let's add the "Contact Us" button inside the paragraph that currently contains the "Learn More" button:

```html
<button type="button" class="btn btn-primary btn-lg" data-toggle="modal" data-target="#myModal">Contact Us</button>
```

Then go test drive that modal! (save, reload, click...)

### Override default text shadows

That modal has an awful text shadow. Let's fix it by overriding some of cover.css's styles in `apprend.css`:

```css
.modal-content {
  color: #333;
  text-align: left;
  text-shadow: none;
}
```

> Don't forget to go back and test it out

# Recap - What Just Happened

We added a version of a stock modal from getbootstrap.com, added a button to trigger it, and overwrote some diagreeable default text styles.

### Check In

Let's compare our in-progress site, to our goal: [apprend.github.io/jquery-bootsrap-workshop/](http://apprend.github.io/jquery-bootsrap-workshop/)

### More Mods - link color

Links should be the color of mustard, in honor of a classic coney dog. To make it happen, add this to `apprend.css`:

```css
a {color: yellow;}
```

### More Mods - Text Protection Scrim

For tripple bonus points, we can add a text protection scrim to make the main copy easier to read:

```css
.cover-container {
  background: radial-gradient(rgba(0,0,0, .7) 0%, transparent 70%);
  text-shadow: 0 1px 2px #000;
}

.cover-container .inner.cover {
    padding: 2em;
}
```

### More Mods - Credits Pt.1

We didn't create any of the images or text used on our sample site. As such, we should credit the authors. These mods are on [http://apprend.github.io/jquery-bootsrap-workshop/](http://apprend.github.io/jquery-bootsrap-workshop/) and can be done on your own time.

Modify the "Learn More" link to point to [http://theeatenpath.com/2009/11/24/coney-island-dogs-american-lafayette-detroit-michigan/](http://theeatenpath.com/2009/11/24/coney-island-dogs-american-lafayette-detroit-michigan/)

### More Mods - Credits Pt.2

Add add this to the footer at the bottom of `index.html` (@`div.mastfoot .inner p`)

```html
Coney by <a href="https://www.flickr.com/photos/52156302@N00/3820831878/in/photostream/">Konrad Maziarz</a>.
Background from <a href="http://en.wikipedia.org/wiki/History_of_Detroit#mediaviewer/File:Michigan_%26_Griswold_circa_1920.jpg">DPL</a>
```

### Further Reading

You'll notice on the demo site, that the "Lafayette Coney Island" link has a tooltip over it. We don't have enough time to build that today, but you should try to do it on your own!



# Closing Thoughts

Holy cow! Look at how much website we got for our effort!

# Thank You!

<img src="http://apprend.org/images/apprend-logo.png" class="logo" alt="Apprend Logo
"/>

Remember to checkout our upcoming events on [apprend.org](http://apprend.org) or [meetup.com/apprend](http://www.meetup.com/apprend/). Also, get your social media on with is:

[apprend.org/](http://apprend.org/) - [@apprenddetroit](https://twitter.com/apprenddetroit)
[facebook.com/apprenddetroit](https://www.facebook.com/apprenddetroit) -  [meetup.com/apprend](http://www.meetup.com/apprend/)
