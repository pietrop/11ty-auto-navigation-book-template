# Performance Checklist

- [ ]  Compress optimise images`ImageOptim`
- [ ]  Image sprite `(?)` | Tool: `SpriteCow`
- [ ]  avoid CSS `@import` to avoid blocking request
- [ ]  Move `<script>` tags to the end of the page.
- [ ]  use `defer` for analytics library
- [ ]  Mark your javascript as deferred or async (?)
- [ ]  Use a CDN (eg Amazon Cloud front)
- [ ]  truncate animate.css to only include the animations we use
- [ ]  Further compress Js. Use webpack gzip
- [ ]  Check your assets
- [ ]  Remove Bootstrap Js & JQuery if not needed
- [ ]  Any unused npm packages we can ditch? (and or tree shaking)
- [ ]  compress splats
- [ ]  Minify CSS
- [ ]  Concatenate your CSS
- [ ]  Minify Javascript
- [ ]  Concatenate your Javascript
- [ ]  Consider Removing polyfills for older browsers to reduce size. If not necessary.

## Notes from a MozzFest session on web performance

# **Web performance optimisation**

## **1 image formates**

Eg SVG for icons and logosJPEG for photosPNG for everything else.

### **1 a. icon fonts**

don’t use it.[iconmoon.io](http://iconmoon.io/) eg get zip file from font awesome

## **2 compress images /optimise images**

SVG: SVGOMGSVG/JPEG/PNG: Compressorosx: ImageOptimlinux: trimagewindows: fileOptimizer

## **3 Use image sprites**

Sprites combine images into a single file.CSS code lets you use the images.

Tool: SpriteCow

## **4 Minify CSS & Javascript**

Minifies for CSS and Javascripteg shorten variable nameseg remove white spaces.Tool: CSS Minifier / Javascript Minifier

## **5 Concatenate your CSS & Javascript**

concat minified CSS and JSimproves HTTP request response time, it’s fewer files.

## **6 avoid CSS @import**

Rather use <link> tag which allows you to download in parallel.rather then as a blocking request

## **7 Move all your <script> tags to the end of the page.**

right before </body> tag. because these are sequentially downloaded

## **8 Mark your javascript as deferred**

<script src="script.js" defer></script>

if you only have one script tag. as it ignores the order

async, keeps the order in which they appear

means don’t stop importing the js code, it continue rendering the page

## **9 Use a CDN**

eg cloud farecontent distribution network

## **10 Check your assets**

you might not need all the js you are usingeg Jquery, might not be needed.

website: you might not need jquery plugins .comwebsite: you might not need jquery .com