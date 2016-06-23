# CSS Foundations

There are heaps of CSS3 goodies and economies that will elevate our responsive design from merely "a normal website made responsive" to a responsive website built for the future. By utilizing CSS3, we will enable our responsive design to load faster, require less resource and be far easier to maintain and amend in the future.

{% raw %}
<video id="videoEmbed" class="video-js vjs-default-skin vjs-16-9 vjs-big-play-centered vjs-fluid" controls preload="auto" data-setup="{}">
  <source src="assets/css.mp4" type="video/mp4">
  <p class="vjs-no-js">To view this video please enable JavaScript, and consider upgrading to a web browser that supports HTML5 video</p>
</video>
{% endraw %}

It makes no difference what text editor or IDE system you use to build your responsive designs. If the simplest of text editors allows you to write your HTML, CSS, and JavaScript efficiently, that's absolutely fine. Similarly there are no requisite pieces of tooling that are essential to get a responsive web design out of the door.

All you actually need is something that enables you to write HTML, CSS, and JavaScript. Whether your preference is Sublime Text, Vim, Coda, Visual Studio, or Notepad - it matters little. Just use what works best for you.

There are more tools available now (often free) to negate many of the manual and time-intensive tasks of building web sites than ever before. For example, CSS processors (Sass, LESS, Stylus, PostCSS) can help with code organization, variables, color manipulations, and arithmetic. Tools like PostCSS can also automate horrible and thankless jobs like CSS vendor prefixing. Furthermore, 'linting' and validation tools can check your HTML, JavaScript, and CSS code against standards as you work, eliminating many time wasting typos or syntax errors.

New tools come out constantly and they are continually improving. We won't be relying on anything other than standards based HTML and CSS in our examples. You should however, use whatever tools you can to produce your front-end code as quickly and reliably as possible.

## The CSS3 Cheat Sheet

The CSS3 cheat sheet defines a list of all the styles in CSS3. It can be used as a reference, as it will be handy while we are writing the CSS3 code. The cheat sheet can be found on the [Smashing Magazine](http://media.smashingmagazine.com/wp-content/uploads/images/css3-cheat-sheet/css3-cheat-sheet.pdf) website.

## A Quick Note on Transitions

Transitions enable us to determine the speed of animation as well as introduce delays, as and when required. They also allow web designers to alter the state and behavior of elements in use.

When we define the transition property along with the state altering properties, only those properties will be undergoing transition. We also need to remember that vendor prefixes have to be used, for example, we'll use `–moz` for Firefox.

Before we move on, have a look at the following example and see if you can mock up a quick HTML demo:

```html
<html>
  <head>
    <style>
    #flex-container {
      display: -webkit-flex;
      display: flex;
      width: 500px;
      height: 500px;
      background-color: Silver;
    }
    #flex-item {
      background-color: lime;
      transition-property: background;
      -webkit-transition-property: background;
      transition-duration: 3s;
      -webkit-transition-duration: 3s;
      transition-timing-function: linear;
      -webkit-transition-timing-function: linear;
      width: 200px;
      height: 200px;
      margin: 20px;
    }
    #flex-item:hover {
      background: red;
    }
    </style>;
  </head>;
  <body>;
    <div id="flex-container">;
      <div id="flex-item">Alpha</div>;
      <div id="flex-item">Beta</div>;
    </div>
  </body>
</html>
```

Don't worry if you get stuck - we'll dive right into the details and just *what* those dashed properties actually do in our next section.
