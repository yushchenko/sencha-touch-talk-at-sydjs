# Sencha Touch + Your Next Project === Love?

## Introduction

Hey, my name is Valery. 
I am a JavaScript developer like many of you here.
At the end of the last year
I had a chance to try how mobile web development looks like
and now I would love to share some of these findings with you.
During next 10 minutes I will give you a short overview of
Sencha Touch JavaScript framework.

In Fairfax, the company where I work,
*some not particularly technical people* call me a 'Sencha developer'.
It sounds ridiculous, in the same way one can address a carpenter
as a 'hammer operator'.

What I am trying to convey here is that a framework or library
is just a **tool** to make job done.
Hopefully, starting a shiny new project you have a **choice**
which particular tool to pick up.

In the real word, nothing is ideal, so even the best tools have its pros and cons.
What is a great for one task or project can be terrible for another.
I am telling these trivial things just for one simple reason.
Considering new, shiny and professionally marketed technology
we need to have proper attitude to have **real choice**
but not just follow the herd.

OK, let move on.

## Mobile vs Desktop

First of all lets take a look how mobile world is different
from good, old and familiar desktop.

> fragment: screen ...

The most obvious difference is screen size.

Screen real estate is precious.
Having 320px width you can forget about many familiar UX patterns
like grids and trees with inline editing.
Obviously we need controls designed **specifically** for mobile.

> fragment: fingers ...

Next, for many people it was a lovely surprise that there is no mouse!
Tap instead of click, swipe instead of scroll and no hover event at all!
**How to live in such terrible world ?!!**

In addition to this we need to handle
such fancy interactions like **pinch** and **rotate**.
Think, the library of our choice should give us a hand here.

> fragment: performance ...

And the next challenge is performance.
Mobile hardware and browsers are optimized for energy saving first.
Unfortately but inevitebly it takes heavy toll on performance.
Yes, phones are getting faster over the time but it still far far away from desktop.
It's not scientificaly precise but it's fairly safe to assume code
on a device will be in 100 times slower than in Google Chrome on your MacBook Pro.

Memory is not in abandance either.
It's fairly easy to slow down even iPhone 4S.
Just let youself to be a little bit relaxed about application's DOM size.

And to make the picture perfect, there is 3G network.
It's not only slow but it can have very long round trip.
One HTTP request can easy take up to 700 miliseconds
and it doesn't matter how fast your server side API is.

> fragment: WebKit...

One more difference here.
It is rather exciting than terrifying.
If you open StatCounter's stats for mobile browsers here in Australia,
you can see that the landscape is dominated by WebKit.
The share of SymbianOS is less than 1% and it's declining.
Well, there is Windows Phone on the horizon.
It is something around 0.8% of all smartphone users now.
Will see how it will be going...

WebKit domination is exciting because it literally means
that you can not only read about HTML5 and CSS3 but also use them.
I personally realy enjoy using CSS3 flex box model.

## Mobile Libraries & Frameworks

> slide

Now lets take a look which libraries are here to make our life easier.

* Sencha Touch
* jQuery + jQuery Mobile + ...
* Zepto.js + ...
* Micro libraries like iScroll
* ...

This list is sorted from top to bottom by amount of features that libraries provide.
Obviously nothing comes without price so library's size increases in the same order.

##  Why Sencha Touch Rocks?

> slide

Class System and MVC

  * inheritance, mixins, statics, singleton
  * automatic dependency management
  * standart application architecture
  * declarative selector based event binding
  * deep linking support (routing)

> slide

Rich Set of Components

  * lists and forms - look and feel close to native
  * toolbars, buttons and icons
  * tabs, carousel and overlays
  * awesome charts (separate component)

> slide

And More Goodness

* Core utils: DOM, selectors, platform detection, templates etc
* themes based on SASS and Compass
* command line tools: scaffolds, build & packaging

## Why Sencha Touch Sucks?

> slide

* supports only iOS, Android and Blackberry at the moment
* complex: learning curve can be high
* heavy: for example 420/142Kb - JS, 133/65Kb - CSS
* not on GitHub

## How to Study

> slide

* Guides, videos and samples
* Samples: KitchenSink
* API docs & source code
* Blog, forum & Twitter
  minor version updates

## Add More Coffeine

> slide: CoffeeScript logo

## Thanks

> slide
