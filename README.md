<p align="center">
  <a href="http://materializecss.com/">
    <img src="http://materializecss.com/res/materialize.svg" width="150">
  </a>
</p>

<h3 align="center">MaterializeCSS</h3>

<p align="center">
  Materialize, a CSS Framework based on material design.
  <br>
  
## Getting Started
### Learn how to easily start using Materialize in your website.

### Download
Materialize comes in two different forms. You can select which version you want depending on your preference and expertise. To start using Materialize, all you have to do is download one of the options below.

Materialize
This is the standard version that comes with both the minified and unminified CSS and JavaScript files. This option requires little to no setup. Use this if you are unfamiliar with Sass. [Materialize](https://github.com/Dogfalo/materialize/releases/download/1.0.0-rc.2/materialize-v1.0.0-rc.2.zip)

Sass
This version contains the source SCSS files. By choosing this version you have more control over which components to include. You will need a Sass compiler if you choose this option. [Sass](https://github.com/Dogfalo/materialize/releases/download/1.0.0-rc.2/materialize-src-v1.0.0-rc.2.zip)


### CDN
You can find all the versions of the CDN at cdnjs.

```js
    <!-- Compiled and minified CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0-rc.2/css/materialize.min.css">

    <!-- Compiled and minified JavaScript -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0-rc.2/js/materialize.min.js"></script>
```            

### NPM
You can also get the latest release using NPM. This release contains source files as well as the compiled CSS and JavaScript files.

```js
    npm install materialize-css@next
```            

### Bower
You can also get the latest release using bower. This release contains source files as well as the compiled CSS and JavaScript files. (bower is deprecated.)

```js
    bower install materialize
```            
### Setup
Project Structure
After downloading, extract the files into the directory where your website is located. Your directory will look something like this.

You'll notice that there are two sets of the files. The min means that the file is "compressed" to reduce load times. These minified files are usually used in production while it is better to use the unminified files during development.

```js
  MyWebsite/
  |--css/
  |  |--materialize.css
  |
  |--fonts/
  |  |--roboto/
  |
  |--js/
  |  |--materialize.js
  |
  |--index.html
```          
### HTML Setup
Next you just have to make sure you link the files properly in your webpage. Generally it is wise to import javascript files at the end of the body to reduce page load time. Follow the example below on how to import Materialize into your webpage.

```js
  <!DOCTYPE html>
  <html>
    <head>
      <!--Import Google Icon Font-->
      <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
      <!--Import materialize.css-->
      <link type="text/css" rel="stylesheet" href="css/materialize.min.css"  media="screen,projection"/>

      <!--Let browser know website is optimized for mobile-->
      <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    </head>

    <body>

      <!--JavaScript at end of body for optimized loading-->
      <script type="text/javascript" src="js/materialize.min.js"></script>
    </body>
  </html>
```        
 
### Third-party Options
There are a few community-made options for you to easily include Materialize in your project. Keep in mind these are untested and may be out-of-date.

### Ruby Gem
See [here](https://github.com/mkhairi/materialize-sass) for documentation on this gem.


 > gem 'materialize-sass'
          
### Meteor Package

  meteor add materialize:materialize
          
### Ember Package
```js
  # install via npm
  $ npm install ember-cli-materialize --save-dev
  # make ember-cli fetch internal dependencies
  $ ember g ember-cli-materialize
```          
### Sass Setup
This section is only relevant if you chose to download the Sass version of Materialize.

### Compiling Sass
Instead of having a css folder, you will find that the download instead contains many .scss files which contain the styles of individual components. Unfortunately, the browser cannot interpret Sass, so you must have your Sass compiler compile the scss/materialize.scss into a regular CSS file. At this point you can link this newly outputted file in your HTML page.

```js
  MyWebsite/
  |--css/
  |  |--materialize.css <-- compiled from scss/materialize.scss
  |
  |--js/
  |  |--materialize.js
  |
  |--scss/
  |  |--materialize.scss
  |  |--components/
  |
  |--index.html
```        
