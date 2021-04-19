<h1>
    <img src="https://cdn.jsdelivr.net/gh/nextapps-de/winbox@master/demo/winbox.svg" alt="WinBox.js: HTML5 Window Manager for the Web." width="100%">
</h1>
<h3>Modern window manager for the web: lightweight, outstanding performance, no dependencies, fully customizable, open source!</h3>

<a target="_blank" href="https://www.npmjs.com/package/winbox"><img src="https://img.shields.io/npm/v/winbox.svg"></a>
<a target="_blank" href="https://github.com/nextapps-de/winbox/issues"><img src="https://img.shields.io/github/issues/nextapps-de/winbox.svg"></a>
<a target="_blank" href="https://github.com/nextapps-de/winbox/blob/master/LICENSE.md"><img src="https://img.shields.io/npm/l/winbox.svg"></a>

<a href="https://nextapps-de.github.io/winbox/">Demo</a> &ensp;&bull;&ensp; <a href="#started">Getting Started</a> &ensp;&bull;&ensp; <a href="#options">Options</a> &ensp;&bull;&ensp; <a href="#api">API</a> &ensp;&bull;&ensp; <a href="#styling">Styling</a> &ensp;&bull;&ensp; <a href="#controls">Controls</a></a> &ensp;&bull;&ensp; <a href="CHANGELOG.md">Changelog</a>

<h3>Live Demo / Code Examples: <br><a href="https://nextapps-de.github.io/winbox/">https://nextapps-de.github.io/winbox/ </a></h3>

<a name="started" id="started"></a>
## Getting Started

<!--
__Version Explanation__

<table>
    <tr>
        <td>Bundle</td>
        <td>
            All assets bundled into one single file (js + css + html + icons).
        </td>
    </tr>
    <tr></tr>
    <tr>
        <td>Non-Bundled</td>
        <td>
            Each asset file exists separately. Recommended when using own bundler.
        </td>
    </tr>
</table>
-->

__Get Latest Build (Stable):__

<table>
    <tr>
        <td colspan=3">
            <b><u>Bundle:</u></b> (all assets bundled into one single file: js + css + html + icons)
        </td>
    </tr>
    <tr>
        <td>winbox.bundle.js</td>
        <td><a href="https://github.com/nextapps-de/winbox/raw/0.0.9/dist/winbox.bundle.js" target="_blank">Download</a></td>
        <td><a href="https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/dist/winbox.bundle.js" target="_blank">https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/dist/winbox.bundle.js</a></td>
    </tr>
    <tr>
        <td colspan=3">
            <br><b><u>Non-Bundled:</u></b> (js and css are separated, css includes icons as base64)
        </td>
    </tr>
    <tr>
        <td>winbox.min.js</td>
        <td><a href="https://github.com/nextapps-de/winbox/raw/0.0.9/dist/js/winbox.min.js" target="_blank">Download</a></td>
        <td><a href="https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/dist/js/winbox.min.js" target="_blank">https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/dist/js/winbox.min.js</a></td>
    </tr>
    <tr></tr>
    <tr>
        <td>winbox.min.css</td>
        <td><a href="https://github.com/nextapps-de/winbox/raw/0.0.9/dist/css/winbox.min.css" target="_blank">Download</a></td>
        <td><a href="https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/dist/css/winbox.min.css" target="_blank">https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/dist/css/winbox.min.css</a></td>
    </tr>
    <tr>
        <td colspan=3">
            <br><b><u>Sources:</u></b> (not bundled at all, images as url to original resources)
        </td>
    </tr>
    <tr>
        <td>ES6 Modules</td>
        <td><a href="https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/nextapps-de/winbox/tree/0.0.9/src/js" target="_blank">Download</a></td>
        <td>The <i>/src/js</i> folder of this Github repository</td>
    </tr>
    <tr></tr>
    <tr>
        <td>winbox.less (source)</td>
        <td><a href="https://github.com/nextapps-de/winbox/raw/0.0.9/src/css/winbox.less" target="_blank">Download</a></td>
        <td><a href="https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/src/css/winbox.less" target="_blank">https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/src/css/winbox.less</a></td>
    </tr>
    <tr></tr>
    <tr>
        <td>winbox.css (compiled)</td>
        <td><a href="https://github.com/nextapps-de/winbox/raw/0.0.9/src/css/winbox.css" target="_blank">Download</a></td>
        <td><a href="https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/src/css/winbox.css" target="_blank">https://rawcdn.githack.com/nextapps-de/winbox/0.0.9/src/css/winbox.css</a></td>
    </tr>
    <tr></tr>
    <tr>
        <td>src.zip</td>
        <td><a href="https://minhaskamal.github.io/DownGit/#/home?url=https://github.com/nextapps-de/winbox/tree/0.0.9/dist" target="_blank">Download</a></td>
        <td>Download all source files including image original resources.</td>
    </tr>
</table>


__Get Latest Build (Nightly):__

Just exchange the version number from the URLs above with "master", e.g.: "/winbox/__0.0.9__/dist/" into "/winbox/__master__/dist".


__Get Latest (NPM):__

```cmd
npm install winbox
```


__Get Latest (ES6 Modules):__

https://github.com/nextapps-de/winbox/tree/master/src/js

### Use Bundled Version

The bundled version includes all assets like js, css, html and icon images as base64.

```html
<html>
<head>
    <script src="winbox.bundle.js"></script>
</head>
<body></body>
</html>
```

### Use Non-Bundled Version

The non-bundled version needs to load js and css separately (css also includes icons as base64).

```html
<html>
<head>
    <link rel="stylesheet" href="winbox.min.css">
    <script src="winbox.min.js"></script>
</head>
<body></body>
</html>
```

### Preload Library / Async Load (Recommended)

Just add a link tag to the header sections which indicated to preload the script. Right before the body is closing add your site scripts. Depending on your code you may need to load them in the right order.

```html
<html>
<head>
    <title></title>
    <link rel="preload" href="winbox.bundle.js" as="script">
</head>
<body>
    <!--
    
    HTML CONTENT
    
    -->
    <!-- BOTTOM OF BODY -->
    <script src="winbox.bundle.js" defer></script>
    <!-- YOUR SCRIPT -->
    <script src="my-script.js" defer></script>
</body>
</html>
```

You can also load the non-bundled version in the same way.

> In rare situations it might produce a short flashing/reflow after page load, depending on your stack. Moving the script tag into the head section will solve this issue. Also try to use the non-bundled version.

### ES6 Modules

The ES6 modules are located in `src/js/`. You need to load the stylesheet file explicitly (includes icons as base64).

```html
<head>
    <link rel="stylesheet" href="dist/css/winbox.min.css">
</head>
```

```html
<script type="module">
  import WinBox from "./src/js/winbox.js";
</script>
```

You can also load modules via CDN, e.g.:

```html
<script type="module">
  import WinBox from "https://unpkg.com/winbox@0.0.9/src/js/winbox.js";
</script>
```

The ES6 modules are not minified. Please use your own bundler for this purpose.

<a name="api"></a>
## Overview

Constructor:

- new <a href="#winbox.new">**WinBox**(title, options\<key: value\>)</a> : winbox

Global methods:

- <a href="#winbox.new">WinBox.**new**(title, options\<key: value\>)</a> : winbox

Instance methods:

- <a href="#winbox.mount">winbox.**mount**(src)</a>
- <a href="#winbox.unmount">winbox.**unmount**(dest)</a>
- <a href="#winbox.move">winbox.**move**(x, y)</a>
- <a href="#winbox.resize">winbox.**resize**(width, height)</a>
- <a href="#winbox.close">winbox.**close**()</a>
- <a href="#winbox.focus">winbox.**focus**()</a>
- <a href="#winbox.minimize">winbox.**minimize**(state)</a>
- <a href="#winbox.maximize">winbox.**maximize**(state)</a>
- <a href="#winbox.fullscreen">winbox.**fullscreen**(state)</a>
- <a href="#winbox.setBackground">winbox.**setBackground**(string)</a>
- <a href="#winbox.setTitle">winbox.**setTitle**(string)</a>
- <a href="#winbox.setTitle">winbox.**setUrl**(string)</a>

Instance properties:

- <a href="#winbox.id">winbox.**id**</a>
- <a href="#winbox.body">winbox.**body**</a>
- <a href="#winbox.min">winbox.**min**</a>
- <a href="#winbox.max">winbox.**max**</a>
- <a href="#winbox.x">winbox.**x**</a>
- <a href="#winbox.y">winbox.**y**</a>
- <a href="#winbox.width">winbox.**width**</a>
- <a href="#winbox.height">winbox.**height**</a>
- <a href="#winbox.top">winbox.**top**</a>
- <a href="#winbox.right">winbox.**right**</a>
- <a href="#winbox.bottom">winbox.**bottom**</a>
- <a href="#winbox.left">winbox.**left**</a>

<a name="options" id="options"></a>
## Options

<table>
    <tr></tr>
    <tr>
        <td>Option</td>
        <td>Values</td>
        <td>Description</td>
    </tr>
    <tr>
        <td>id</td>
        <td>number | string</td>
        <td>Set a unique id to the window. Used to define custom styles in css, query elements by context or just to identify the corresponding window instance.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>title</td>
        <td>string</td>
        <td>The window title.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>mount</td>
        <td>HTMLElement</td>
        <td>Mount a element (widget, template, etc.) into the window body.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>html</td>
        <td>string</td>
        <td>Set <code>innerHTML</code> of the window body.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>url</td>
        <td>string</td>
        <td>Open URL inside the window (iframe).</td>
    </tr>
    <tr></tr>
    <tr>
        <td>width<br>height</td>
        <td>number | string</td>
        <td>Set the initial width/height of the window (supports units "px" and "%").</td>
    </tr>
    <tr></tr>
    <tr>
        <td>x<br>y</td>
        <td>number | string</td>
        <td>Set the initial position of the window (supports "center" and also units "px" and "%").</td>
    </tr>
    <tr></tr>
    <tr>
        <td>max</td>
        <td>boolean</td>
        <td>Automatically toggles the window into maximized state when created.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>top<br>right<br>bottom<br>left</td>
        <td>number | string</td>
        <td>Set or limit the viewport of the window available area (supports units "px" and "%").</td>
    </tr>
    <tr></tr>
    <tr>
        <td>modal</td>
        <td>boolean</td>
        <td>Show the window as modal.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>onmove</td>
        <td>function(x, y)</td>
        <td>Callback triggered when the window moves. The keyword <code>this</code> inside the callback function refers to the corresponding WinBox instance.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>onresize</td>
        <td>function(width,&nbsp;height)</td>
        <td>Callback triggered when the window resizes. The keyword <code>this</code> inside the callback function refers to the corresponding WinBox instance.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>onclose<br>onfocus<br>onblur</td>
        <td>function()</td>
        <td>Callbacks to several events (Note: the event 'onclose' will be triggered right before closing). The keyword <code>this</code> inside the callback function refers to the corresponding WinBox instance.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>background</td>
        <td>string</td>
        <td>Set the background of the window (supports all CSS styles which are also supported by the style-attribute "background", e.g. colors, transparent colors, hsl, gradients, background images)</td>
    </tr>
    <tr></tr>
    <tr>
        <td>border</td>
        <td>number</td>
        <td>Set the border width of the window.</td>
    </tr>
    <tr></tr>
    <tr>
        <td>classname</td>
        <td>string</td>
        <td>Add one or more classnames to the window (multiple classnames needs separated with whitespaces, e.g. "class-a class-b"). Used to define custom styles in css, query elements by context or just to tag the corresponding window instance.</td>
    </tr>
</table>


## Examples

<a name="winbox.new" id="winbox.new"></a>
#### Basic Window

> When no `root` was specified the window will append to the `document.body`.

```js
new WinBox("Window Title");
```

Alternatively:
```js
WinBox.new("Window Title");
```

Alternatively:
```js
new WinBox({ 
    title: "Window Title" 
});
```

Alternatively:
```js
var winbox = WinBox();
winbox.setTitle("Window Title");
```

#### Custom Root

```js
new WinBox("Window Title", {
    root: document.body
});
```

#### Custom Color

> Supports all CSS styles which are also supported by the style-attribute "background", e.g. colors, transparent colors, hsl, gradients, background images.

```js
new WinBox("Custom Color", {
    background: "#ff005d"
});
```

Alternatively:
```js
var winbox = new WinBox("Custom Color");
winbox.setBackground("#ff005d");
```

#### Custom Border

```js
new WinBox({
    title: "Custom Border",
    border: 4
});
```

####  Custom Viewport

> Define the available area (supports units "px" and "%").

```js
new WinBox("Custom Viewport", {
    top: "50px",
    right: "5%",
    bottom: 50,
    left: "5%"
});
```

Alternatively (does not support units!):
```js
var winbox = new WinBox("Custom Viewport");

winbox.top = 50;
winbox.right = 50;
winbox.bottom = 50;
winbox.left = 50;
```

#### Custom Position / Size

> Supports units "px" and "%". Also support the keyword "center" for xy-position.

```js
new WinBox("Custom Viewport", {
    x: "center",
    y: "center",
    width: "50%",
    height: "50%"
});
```

Alternatively (also supports units):
```js
var winbox = new WinBox("Custom Viewport");

winbox.resize("50%", "50%")
      .move("center", "center");
```

Alternatively (does not support units!):
```js
var winbox = new WinBox("Custom Viewport");

winbox.width = 50;
winbox.height = 50;
winbox.resize();

winbox.x = 50;
winbox.y = 50;
winbox.move();
```

#### Modal Window

```js
new WinBox({
    title: "Modal Window",
    modal: true
});
```

#### Set innerHTML

```js
new WinBox("Set innerHTML", {

    html: "<h1>Lorem Ipsum</h1>"
});
```

Alternatively:
```js
var winbox = new WinBox("Set innerHTML");

winbox.body.innerHTML = "<h1>Lorem Ipsum</h1>";
```

#### Mount DOM (Cloned)

> By cloning you can easily create multiple window instances of the same content in parallel.

```html
<div id="content">
    <h1>Lorem Ipsum</h1>
    <p>Lorem ipsum [...]</p>
</div>
```

```js
var node = document.getElementById("content");

new WinBox("Mount DOM", {

    mount: node.cloneNode(true)
});
```

Alternatively:
```js
var node = document.getElementById("content");
var winbox = new WinBox("Mount DOM");

winbox.mount(node.cloneNode(true));
```

#### Mount DOM (Singleton) + Auto-Unmount

> A singleton is a unique fragment which can move inside the document. When creating multiple windows and mounting the same fragment to it, the fragment will leave the old window (see the method above for cloning).

You can simply use a hidden backstore to hold contents, as well you can use any other strategy like a templating engine etc.

```html
<div id="backstore" style="display: none">
    <div id="content">
        <h1>Lorem Ipsum</h1>
        <p>Lorem ipsum [...]</p>
    </div>
</div>
```

```js
var node = document.getElementById("content");

new WinBox("Mount DOM", {
    mount: node
});
```

> Auto-Unmount is a great feature which automatically moves back the fragment to the backstore source when closing the window.

Alternatively:
```js
var node = document.getElementById("content");
var winbox = new WinBox("Mount DOM");

winbox.mount(node);
```

#### Explicit Unmount

```html
<div id="backstore" style="display: none">
    <div id="content">
        <h1>Lorem Ipsum</h1>
        <p>Lorem ipsum [...]</p>
    </div>
</div>
<div id="backstore-2" style="display: none"></div>
```

```js
var node = document.getElementById("content");
var winbox = new WinBox("Mount DOM");
```

Move fragment from hidden backstore to the window body:

```js
winbox.mount(node);
```

Move fragment back to the hidden backstore source:

```js
winbox.unmount();
```

Or move fragment to another destination:

```js
winbox.unmount(document.getElementById("backstore-2"));
```

Or just auto-unmount as default when closing:

```js
winbox.close();
```

Override default auto-unmount behavior when closing the window:

```js
new WinBox("Mount DOM", {
    mount: node,
    onclose: function(){
        this.unmount(document.getElementById("backstore-2"));
    }
});
```

#### Manual Mount

Feel free to use the `winbox.body` directly:
```js
var node = document.getElementById("content");
var winbox = new WinBox("Mount DOM");

winbox.body.appendChild(node);
```

Or delegate it as a root to your templating engine, e.g.:
```js
Mikado(template).mount(winbox.body).render(data);
```

#### Open URI / URL

> You can use every URI scheme which is supported by `src` attribute, e.g. URL, image or video, base64 encoded data.

```js
new WinBox("Open URL", {
    
    url: "https://wikipedia.com"
});
```

Alternatively:
```js
var winbox = new WinBox("Open URL");

winbox.setUrl("https://wikipedia.com");
```

#### The Window Instance

```js
var winbox = new WinBox();

console.log("Window ID:", winbox.id);
console.log("Current Position X:", winbox.x);
console.log("Current Position Y:", winbox.y);
console.log("Current Width:", winbox.width);
console.log("Current Height:", winbox.height);
console.log("Current Maximize State:", winbox.max);
console.log("Current Minimize State:", winbox.min);
```

#### Controls

```js
var winbox = new WinBox();
```

Focus a window (bring up to front):
```js
winbox.focus();
```

Toggle the minimized state of a window:
```js
winbox.minimize();
```

Explicitly set the minimized state of a window:
```js
winbox.minimize(true);
winbox.minimize(false);
```

Toggle the maximized state of a window:
```js
winbox.maximize();
```

Explicitly set the maximized state of a window:
```js
winbox.maximize(true);
winbox.maximize(false);
```

Toggle the fullscreen state of a window:
```js
winbox.fullscreen();
```

Explicitly set the fullscreen state of a window:
```js
winbox.fullscreen(true);
winbox.fullscreen(false);
```

Close and destroy a window:
```js
winbox.close();
```

#### Chaining Methods

```js
var winbox = WinBox();

winbox.setTitle("Title")
      .setBackground("#fff")
      .resize("50%", "50%")
      .move("center", "center")
      .mount(document.getElementById("content"));
```

> When using "center" as position you need to call `resize()` before `move()`.

## Customize Window

The window boilerplate:

<img src="https://cdn.jsdelivr.net/gh/nextapps-de/winbox@master/demo/boilerplate.svg?v=4" width="100%" alt="WinBox Boilerplate">

Hide or disable specific icons:

```css
.wb-min   { display: none }
.wb-full  { display: none }
.wb-max   { display: none }
.wb-close { display: none }
```

Hide or disable all icons:

```css
.wb-icon { display: none }
```

Modify a specific icon:

```css
.wb-max {
    background-image: url(src/img/max.png);
    background-position: center;
    background-size: 15px auto;
}
```

Disable resizing areas:

```css
/* north */
.wb-n  { display: none }

/* east */
.wb-e  { display: none }

/* south */
.wb-s  { display: none }

/* west */
.wb-w  { display: none }

/* north-west */
.wb-nw { display: none }

/* north-east */
.wb-ne { display: none }

/* south-west */
.wb-sw { display: none }

/* south-east */
.wb-se { display: none }
```

Disable or modify the window drop shadow:
```css
.winbox { box-shadow: none }
```

Style the window background:
```css
.winbox {
    background: linear-gradient(90deg, #ff00f0, #0050ff);
    border-radius: 12px 12px 0 0;
}
```

Style the header title:
```css
.wb-title { font-size: 12px }
```

Style the body of a window element incl. the window border:
```css
.wb-body {
    /* the width of window border: */
    margin: 4px;
    color: #fff;
    background: #131820;
}
```

> The margin of `.wb-body` corresponds to the width of the window border.

Apply styles when window is in "minimized" state:
```css
.winbox {
    border-radius: 10px;
}
.winbox.min {
    border-radius: 0;
}
.winbox.min .windbox-title {
    font-size: 12px;
}
```

Apply styles when window is __not__ in "minimized" state:
```css
.winbox:not(.min) {
    /* apply styles */
}
```

Apply styles when window is in "maximized" state:
```css
.winbox {
    border-radius: 10px;
}
.winbox.max {
    border-radius: 0;
}
.winbox.max .wb-max {
    opacity: 0.5;
}
```

Apply styles when window is __not__ in "maximized" state:
```css
.winbox:not(.max) {
    /* apply styles */
}
```

Apply styles when window is in "fullscreen" state:
```css
.wb-body:fullscreen {
    /* apply styles */
}
```

Apply styles when window is in "focus" state:
```css
.winbox {
    background: #999;
}
.winbox.focus {
    background: #0050ff;
}
.winbox .wb-icon {
    display: none;
}
.winbox.focus .wb-icon {
    display: block;
}
```

Apply styles when window is __not__ in "focus" state (the same logic from example above, but shorter):
```css
.winbox:not(.focus) {
    background: #999;
}
.winbox:not(.focus) .wb-icon {
    display: none;
}
```

Apply styles when window is in "modal" state:
```css
.winbox.modal .wb-close { display: none }
```

Customize the modal background overlay:
```css
.winbox.modal:after{
    background: #0d1117;
    opacity: 0.5;
    animation: none;
}
```

## Useful Examples

> Without the header the user isn't able to move the window frame. Instead, you can place your own control elements to the page.

Always hide the window header:

```css
.wb-header { display: none }
.wb-body   { top: 0 }
```

Hide the header just in maximize mode:

```css
.winbox.max .wb-header { display: none }
.winbox.max .wb-body   { top: 0 }
```

---


Copyright 2021 Nextapps GmbH<br>
Released under the <a href="http://www.apache.org/licenses/LICENSE-2.0.html" target="_blank">Apache 2.0 License</a><br>
