# Vanilla.js image modal gallery

![Requires.io (branch)](https://img.shields.io/requires/github/konfer-be/kbox/master)
![Snyk Vulnerabilities for GitHub Repo](https://img.shields.io/snyk/vulnerabilities/github/konfer-be/kbox)
[![GPL Licence](https://badges.frapsoft.com/os/gpl/gpl.svg?v=103)](https://opensource.org/licenses/gpl-license.php)

Simple image modal gallery in pure vanilla.js.
        
## > Demo

https://demo.konfer.be/kbox/

## > Install

``` bash
> $ npm install kbox --save
```

## > How to use ?

In your HTML page, between <head> tags, retrieve styles:

``` html 
<link href="css/kbox.css" rel="stylesheet" type="text/css" media="screen" />
```

And link kbox pack script (contains velocity.js and kbox.js as packaged solution) :

``` html 
<script type="text/javascript" src="js/kbox.pack.min.js"></script>
```

Puts the kbox class on the links where you will place your images, and replace data attributes values with your own values :

``` html 
<a class="kbox" data-kbox="Travels"> <img src="url-to-your-img.jpg" alt="" /> <a>
```

Note the data-kbox attribute, which determine the gallery collection of the picture.
 
An then, invoke the plugin :

``` javascript
window.kbox();
```

## > I18n

Kbox display interface text contents in the following languages : french, english, dutch, german, italian, spanish, polish and russian. 

If your language is not supported, create your own locale file and do a pull request !
    
## > Dependencies 

Kbox uses [velocity.js](http://velocityjs.org/) to display progressive animations. If you have already linked velocity.js in your project, import the kbox.min.js file instead of kbox.pack.min.js. 

Kbox uses also hody-icons font icon, packaged into the project.

## > Options

Following options are available :

* **lang**: string, lang catalog to use
* **animationSpeed**: int, speed of the transition animation (ms)
* **keyboard**: boolean, using keyboard navigation
* **titles**: boolean, display titles attributes
* **afterOpening**: function(e), function, callback fired after modal opening
* **afterTransition**: function(e), function, callback fired after image display transition
* **afterClosing**: function(e), function, callback fired after modal closing

## > Licence

[GPL](https://opensource.org/licenses/gpl-license.php)
