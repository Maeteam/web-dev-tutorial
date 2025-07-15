# Web Development Tutorial
```
Description:
while playing this game I discovered a bunch of cool methods and functions to create an awesome website,
then i decided to make it open source to allow other players to create awesome websites.
```
a tutorial for web development in a single html file, including javascript and css. this tutorial is for grey hack the game but could also be applied to real html web development
# This project is for a game
<br>[Grey hack on steam](https://store.steampowered.com/app/605230/Grey_Hack/)
## Table of Contents
- [The basics](#html-basics)
- [Cheat Sheet](#Cheat-Sheet)
- [Examples](#examples)
- [Cascade Style Sheets](#Cascade-style-sheets)
- [Creating shops](#Creating-shops)
- [ID cheatsheet](#id-cheatsheet)
- [Load images](#load-images)
- [Javascript](#javascript)
- [Mouse whell scrolling](#Mouse-wheel-scrolling)
## HTML basics
HTML works in a simple way,<br>
you have built-in "classes", some example ones are:
- Paragraph
- Headline
- Bold

<br>Those are pretty straightforward,<br>
To set up a starting point, every "object" is surrounded by angle brackets,<br>
or `<>`, so for example:
`<Start-paragraph>Hello!<end-paragraph>`<br>
Note: this isnt actual syntax, its just an example.<br>
how you would actually proceed would be like so:<br>
```html
<p>Hello world!</p>
```
<b><b>Note: `<p>` is for paragraph</b><br>
Now, you could see you start by doing `<p>`, to indicate you want a paragraph.<br>
and `</p>`, notice the slash P, indicating to end the paragraph.

## Cheat Sheet
| Type       | Description     |
|------------|----------------|
| `<p>`     | Paragraph       |
| `<b>`        | Bold       |
| `<br>`    | Newline |
| `<h>`      | Header |
| `<i>`      | Italic |
| `<button>`      | Button class |
| `<div>`      | generic container |
<br>
Notice: a lot of real life html classes don't work inside grey hack.<br>
but search actual html on google and try things out, thats how you find out new things!.
```
Fun fact: <br> doesnt need closing, its basically like using \n in coding
just do <br> without </br> and it will go down a line without causing problems!
```

## Examples
[Example Scripts](Example-Sources)
[Default Templates](Example-Sources/Default-templates)
## Cascade style sheets
Alright, so cascade style sheets.<br>
lets start simple, cascade styling sheets, or `css`, is "kinda" a programming language<br>
since it is inside of html but people usually choose to add an additional file called `style.css`.<br>
Now, its important to know some of css' features in real html don't apply to grey hack.<br>
BUT, unlike html & javascript, css is probably the most similar to real life css, which is great news.<br>
### so, what is cascade style sheets?
remember those classes?, paragraphs & headlines?, then cascade is basically what `Defines`<br>
those classes, it's syntax is like so:
```css
h1 {
  color: #ffffff;
}
.customclass {
  color: #ffffff;
}
```
`NOTE: WHEN USING 'CSS' IN THE SAME FILE AS HTML, YOULL NEED TO SURROUND IT WITH A <style></stlye>`<br>
Now, you might ask, why does customclass have a dot behind it?<br>
great question, customclass is an ACTUAL class, while h1 is more of a "Type"<br>
so if you would want a header that is customclass you would do like so:
```html
<h1 class="customclass">Cool White header</h1>
```
now, this doesnt do anything because both do the same but you could make your life easier with cascade style sheets!<br>
dont worry if you didnt understand it i will continue to talk about it, this is just an introduction<br>
Note that at the end of a setting in css you should put a ";" to end the line, similar to csharp.
<br>`Most css settings are pretty straightforward, but i suggest using google to learn more advanced methods`
## Creating shops
Grey hack has built in IDs for shops, and more websites.<br>
you might be familiar with the hackshop or shop or the bank website<br>
all of these are easily summonable using their ID
```html
<h>My Shop</h>
<p>Buy anything you want, feel free to look into our stock!</p>
<button class="btn btn-primary" id="InformaticaShop">Shop</button>
```
Note: keep in mind the uppercase letters<br>
So, InformaticaShop is calling for the normal shop, a cool thing is, you can actuall run this 3 liner and have a shop up and running<br>
not very good looking, but a shop, so you may ask, where are the files, since you dont see the files in the shop.<br>

### Adding Files to your shop
quick tutorial time!
1. Find the `/server/httpd.conf` file, now a sample description is there, with the classic JSON format, pretty intuitive.
2. now find the `/Public/htdocs/downloads/` folder, there you  put the files, a txt a binary, anything you want.
3. set the name, price and description to your likings.
4. BOOM you have a full shop with an HTML page.

easy peasy<br>
now all we have to do is decorate the website and we are good to go!
## ID Cheatsheet
Remember, IDs are set after the type like so:
`<type class="classname" id="ID">`
| ID       | Description     |
|------------|----------------|
| InformaticaShop     | The classic green shop       |
| RegisterBank        | Register Page to a bank       |
| LoginBank    | Bank login page |
| ISPConfig      | Internet service provider page |
| CreateCurrency      | coin creation page |
| FindDeviceManual      | Device manual finding page |
| JobsPolice      | Police jobs page |
| Report      | Police report suspect page |
| HackShopTools      | Hackshop downloads page |
| HackShopExploits      | Hackshop exploits page |
| Jobs      | Hackshop jobs page |
| CTF      | Hackshop CTF page |

Note: IDs should only belong to one object, it will be cleaner that way.
## load images
lets start off, by saying images are loadable by default in grey hack, but only a few. you can see how to load images in [Default Templates](Example-Sources/Default-templates)
there is a custom way to upload your own images and that i wont cover because i am not that good at it and its messy<br>
but simple image loading
```html
<img src="bank.png" width="120" height="120" align="center">
```
yep, thats it, only src can equal whatever you want, go hunt the web for available pictures, and you can also see them in [Default Templates](Example-Sources/Default-templates)<br>
where almost every page has its own image
## Javascript
okay, so javascript is VERY similar to css, in terms of how it works within the confines of grey hack.<br>
lets start by saying that still, the javascript & html & css are in *the same file*,<br>
javascript, needs a ";" aswell on most of the line ends.<br>
also needs to be surrounded by a `<script></script>`.<br>
simple variable managment include:
```javascript
var _str = "Javascript";
var _num = 99;
```
var & `const` and `let` **can** both be used for string & integers.<br>
i 99% use var since i dont use variable that much but when i do, i use `var`<br>
the differences are minor between the three, but i encourage you to play with them and see what fits you best.<br>
### Functions:
functions are one of the best things in grey hack's web development.<br>
all because of: onclick()<br>
this allows you to create basically everything, your own pages, retractable articles, one of the classiest examples of all the principles learned here are:<br>
### www.gbi.com - in game website!
which i designed their webpage.<br>
Now lets get to work on functions!<br>
```javascript
<button class="accordion" onclick="togglePanel('panel1')">Website seizure - www.buystuff.net</button>
    <div id="panel1" class="panel">
        <p>GBI agents coordinated to save a foreign website that was hacked by malicious actors, now in lockdown until owner claims it. if you are the owner of www.buystuff.net please contact us!</p>
    </div>
<script>
function togglePanel(panelId) {
    var panel = document.getElementById(panelId);
    if(panel.style.display == "block") {
      panel.style.display = "none";
    } else {
      panel.style.display = "block";
    }
  }
</script>
```
### YIPEE!!!
WE HAVE A WORKING TOGGLEABLE PARAGRAPH!<br>
straight taken out of the gbi website, but wait, why does this look so funky in grey hack?<br>
easy answer: cascade style sheets, we didnt include the css in this code snippet, which causes all of the objects to look like the default look<br>
if you would have added a simple snippet like this above:
```css
<style>
.accordion {
      background-color: #1a2f4f;
      color: #e3e3e3;
      cursor: pointer;
      padding: 12px;
      width: 100%;
      text-align: left;
      border: none;
      font-size: 15px;
      margin-top: 10px;
    } 
.accordion:hover{
  background-color: #2b4d77;
}
.panel {
  background-color: #102033;
  display: none;
  padding: 10px;
  border-left: 3px solid #2b4d77;
  border-right: 3px solid #2b4d77;
  border-bottom: 3px solid #2b4d77;
    }
</style>
```
look familiar? cause it is!! its literally the GBI code!
Notice that .accordion has a dot behind it! its a class!!<br>
and in the code we have `<button class="accordion"...`, we set the class to accordion! and we put a dot behind it!<br>
### AWESOME!
now play with this by youself, check out the source files i put in `Example Sources`
## Mouse Wheel Scrolling
### And now, for the thing youve been waiting for..<br>
### Javascript mouse wheel scrolling!!
lets get started!<br>
first of all, i left a template project with scrolling here -> [Source code](Example-Sources/MouseWheelScrolling.html)
check out [Examples](Example-Sources) to see all templates i left in the project!.<br>
now for coding!<br>
alright so lets start by logic, we want the javascript to *listen* to mouse wheel scrolling and then act accordingly,<br>
so lets start, by writing our `<script>`<br>
and setting our scroll speed, basically how fast we travel using the mouse wheel,<br>
an ideal speed would be 0.1, but since its grey hack we need people to appreciate the scroll wheel, and the page is tiny so we need it to not jump.<br>
the best outcome ive seen is `0.05`, do you remember how to set variable?
```javascript
<script>
var scrollSpeedFactor = 0.05;
</script>
```
thats right!, we use var, lets pace things up.<br>
so we want to get *where* to scroll, simple<br>
`var scrollDiv = document.getElementById("scrollArea");`
this line sets a variable, this is exactly the reason why you should only use ID for 1 object,
get **element**, and scrollArea is where you put all the content like so:<br>
```html
<div id="scrollArea"> // set where to scroll
  <div class="content">
    <h>Title</h>
    <p>Line 1</p>
    <p>Line 2</p><br>
  </div>
</div>
```
so, we have scrollArea set up as the ID for the container<br>
scrollDiv will be set to this element. now lets listen for scrolling,
we call for scrollDiv the variable that we just set, and we add listener.<br>
```javascript
scrollDiv.addEventListener("wheel", handleScroll);
```
HOLD UP! not so fast, lets go one by one, so scrollDiv.addEventListener, is pretty straightforward, now "wheel", is simply the mouse wheel<br>
but what is handleScroll? answer: nothing.<br>
its a function which we have yet to create, so lets do!<br>
```javascript
function handleScroll(event) {
  // nothing yet
}
scrollDiv.addEventListener("wheel", handleScroll);
```
alright, looking promising, lets continue,<br>
time for some math - if you dont understand, thats 100% alright, its complicated.<br>
however, i will explain.
```javascript javascript
<script>
var scrollDiv = document.getElementById("scrollArea");
var scrollSpeedFactor = 0.05;
function handleScroll(event) {
  var delta = event.deltaY; // built in function
  var scrollAmount = delta * scrollSpeedFactor; // we set scrollspeedfactor before.
  var newScrollTop = scrollDiv.scrollTop + scrollAmount; // current scroll position
  var maxScrollTop = 440; // how down you can scroll, adjustable
  if (newScrollTop < 0) newScrollTop = 0; // restrict from going too much up
  if (maxScrollTop > 0 && newScrollTop > maxScrollTop) newScrollTop = maxScrollTop; // restrict from going too much down
  scrollDiv.scrollTop = newScrollTop; // scroll position
}
scrollDiv.addEventListener("wheel", handleScroll); // lastly, listen and call handleScroll
</script>
```
a-w-e-s-o-m-e.<br>
so a few things, first of all, maxScrollTop is adjustable, this means youll need to adjust it to the needs of your page, second<br>
you should probably use overflow: hidden; on body like so:
```css
html, body {
  overflow: hidden;
        }
```
that way the normal scroll bar wont appear and cause problems.
<br>Thats about it for mouse wheel scrolling! enjoy this feature!<br>

