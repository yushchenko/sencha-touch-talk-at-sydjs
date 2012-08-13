# Sencha Touch + Your Next Project === Love?

## Introduction

Hey, my name is Valery. 
I am a JavaScript developer like many of you here.
At the end of the last year
I had a chance to try how mobile web development looks like
and now I would love to share some of these findings with you.
During next 15 minutes I will give you a short overview of
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

Screen's real estate is precious.
Having 320px width you can forget about many familiar UX patterns
like grids and trees with inline editing.
Obviously we need controls designed **specifically** for mobile.

> fragment: fingers ...

Next, for many people it was a lovely surprise but there is no mouse!
Tap instead of click, swipe instead of scroll and no hover event at all!

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
and it doesn't matter how fast your server is.

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
in combination with jQuery Mobile.

Lets go futher. 

> fragment: Zepto.js + ...

There is a lightwheight counterpart of jQuery called Zepto.js.
This library is built specifically for mobile devices which run WebKit browsers.

It's much smaller than jQuery and obviously provides less features.
You can use Zepto.js on its own,
in this case you don't have widget and themes like with jQuery Mobile
but only HMTL and CSS in your hands.
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
 
First of all, it's MVC.

> fragment: MVC

Here we have rich data model, views and controllers that glue everything together.

MVC is based on Sencha's class system.

> fragment: rich class system

The class system is shared in between Ext JS -
it's another Secha's library used to build desktop web application -
and Sencha Touch.

It supports classes, mixins, singletons
as well as my favorite feature - dependency management

> fragment: dependency management

Dependency management it's where Sencha Touch really rocks.
How it works? Simple.
When you create an application just tell Sencha
which controllers and views you are using
and all this code will be loaded when you debug and included into build.
Next, lets assume that you inherit a view from Sencha Container component.
This component's source will be loaded and included into build either.
Everything what goes into build is determined only by dependencies
and it's doesn't matter if it's your code or frameworks' code.
In any case you will end up with only code which is really used.

Next my favorite feature is Sencha's deep linking.

> fragment: deep linkig support

Essential part of controller's code it's just event handling.
In sencha it's done in a declarative way.
You provide a selector to determine set of components which events
you want to listen, and event name followed by controller's method name
which will handle the event.
Near the same happens with deep linking: you type URL pattern and controller's
method name and it just works.

> fragment: ...

Then next area where Sencha Touch is really stands out it's components.
Lets take a glance what we have here.

> slide: lists ...

First, it's provides list and forms which look and feel quite close to native.
If you try them on you phone, you will see that the interections
are fairly decent but not perfect, espessialy in comparison with native apps.
In fact, this little slugishness just the price that you pay for the previledge to run
the same code accross different platforms.

> slide: toolbars ...

Next, there are toolbars, buttons and huge set of icons.

> slide: tabs, ...

To put more stuff on small screen we can use tabs, carousels
and various types of overlays.

> slide: awesome charts...

And the brightest comes at the end - we have awesome charts.

> slide: and more goodness

And there are more goodness.

> fragment: selectors

Selectors.
In Sencha you can query DOM using selectors pretty much in the same way as in jQuery.
This is not particularly useful here because you rarely deal with DOM directly,
your code mainly interacts with more high level components.
So in Sencha we have the second type of selectors which work against component tree.
The syntax is pretty much the same so can you them straight away.

> fragment: clientside templates

To build custom components you will need to generate markup
required for their visual representation.
Sencha provides fully functional cliendside templates
to make your life easier.

> fragment: themes

Themes is the next feature worth mentioning.
It is based on SASS and Compass framework.
There are several very decent themes provided with library
and it's fairly easy to generate new ones just tweaking SASS variables.

> fragment: command line

And the last in this "Rock" list is sencha commandline tool.
When you start a new project it will generate scaffolds.
When the project is ready to deploy it will
will walk through the dependencies and combine and crunch
only code that you really use.
It's also possible to wrap your app into native code
if it should be deployed into Apple Store and Google Play.

Now when we have seen some Sencha's strong sides
lets move on to question number two.

## Why Sencha Touch Sucks?

> fragment: <blink>...

First of all it supports only iOS, Android and the latest Blackberries.
At the current version there is no support for Symbian and Windows Phone.
For local australian market it can be fine but if you have customers
for example in China than Sencha Touch simply is not an option for you.

> fragment: 420Kb

Next, Sencha Touch apps are pretty heavy.
For my last project built produces 420 Ks of crunched JavaScript and 133 Ks of CSS.
It is not a small amount to parse for mobile browser
and it is not particulary fast to trasfer it over 3G network.

> fragment: hard to study

Next, it can take some time to study Sencha Touch.
A developer who got used to jQuery often thinks in such way:
I will build my markup first and then I add a pluggin
here to create a nice menu and another pluggin there for a carousel...
This approach works pretty well when you are building a web site.

With Senha you walk in exactly opposite direction -
initially there is no markup at all,
you build component hierarchy first and then each component
generates all markup required for visual representation.

> fragment: not on GitHub

At the end, the last but important thing to mention is Sencha's lisensing.
There is dual license scheme: you can get the framework
under GPL version 3 or under Sencha's own "Free Commercial" lisense.
This "Free Commercial" lisense is not equal to normal MIT license.
For Sencha you are getting the source code but it's not on GitHub
as most of other JavaScript libraries nowdays.

OK, lets suppose that you have decided that 
Sencha Touch rather rocks than sucks
and you want to start using it today.

## How to Study

> fragment: tutorials

First of all I would advise you to open up docs.sencha.com in your browser
and walk through the tutorials.
The tutorials come in two forms - articles and videos.
If you have time read and watch both they cover the same topics
but from different perspective, they are not equivalent.

> fragment: KitchenSink

Next I would go to examples and open up Kitchen Sink application.
In fact, it's rather a directory
which contains examples of most typical Sencha's use cases..
At the right top corner there is the button named "Source",
using it you can take a look at typical configuration of various components.
Or if you are lazy like me, you can just copy paste some code into your app.

> fragment: API docs

During development you will be mainly using API documentation.
It's pretty much comprehensive and contains a lot of examples 
but from time to time you still will want to digg into
framework's source code.

> fragment: source

You can do this right in browser, just put mouse pointer over class name
in API docs and you will see "View source..." link hidden by default.

> fragment: @

The last but not least.
Sencha notifies you about major releases via blog
but it's not so with bug fix and beta releases.
These notification come through their developers forum.
If you are not too much excited about forums,
another way to get these notifications is Twitter
via for example Jamie Avins who works in Sencha's dev team.

## Thanks

OK, it's pretty much all about Sencha, projects and love for today.
Thank you for your patience and time.

[@yushchenko](https://twitter.com/vyushchenko)
