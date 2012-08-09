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

Now let take a look how we can make our life easier.

## Mobile Libraries & Frameworks

This talk about Sencha Touch so it naturally comes first.

> fragment: Sencha...

Arguably, it is the most comprehensive solution for building mobile web app
currently available on the market.
Sencha Touch is great but at the same time it's the haviest
and the most complex option.

> fragment: jQuery + ...

Next alternative is jQuery combined with jQuery Mobile.
These two will do amazing job for you if you are building a mobile web site
and not too much concerned about library size.
But if you are after one page mobile web application,
it would be prudent to employ an MVC framework like Backbone.js or Spine
in combination with jQuery Mobile.x

Lets go futher. 

> fragment: Zepto.js + ...

There is a lightwheight counterpart of jQuery Mobile called Zepto.js.
This library is built specifically for mobile devices which run WebKit browsers.

It's much smaller than jQuery Mobile and obviously provides less features.
For example, with jQM you get quite rich set of widgets
but using Zepto.js you will have only HTML and CSS in your hands.
This approach doesn't look easy but your app is going to be quite lean.

Another option is to combine Zepto.js with jQTouch to get widgets and themes.
In the same way as with jQuery Mobile you would want to use an MVC framework
to structure your code.

> fragment: ...

This list is definetively not complete.
Mobile web landscape is fairly reach and changing quickly.
So you can consider this rather as a starting point for you own research.

OK, let go back to Senha Touch and try to answer a couple of simple questions.

The first one is ...

##  Why Sencha Touch Rocks?

Lets start from ...

> fragment: Application architecture

> fragment: MVC

> fragment: rich class system

> fragment: dependency management

> fragment: deep linkig support

> fragment: ...

> slide: lists ...

> slide: toolbars ...

> slide: tabs, ...

> slide: awesome charts...

> slide: and more goodness

> fragment: selectors

> fragment: clientside templates

> fragment: themes

> fragment: command line

## Why Sencha Touch Sucks?

> fragment: <blink>...

> fragment: 420Kb

> fragment: hard to study

> fragment: not on GitHub

## How to Study

> fragment: tutorials

> fragment: KitchenSink

> fragment: API docs

> fragment: source

> fragment: @

## Thanks

[@yushchenko](https://twitter.com/vyushchenko)
