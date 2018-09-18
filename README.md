# Use less Javascript - ask me how!

These are the speaker notes / outline for the presentation. The deck was created with [Reveal.js](http://lab.hakim.se/reveal-js) and can be found in the [`/deck`](deck) folder.

## Who am I?

* Fabio Neves
* Brazilian by accident, Canadian by choice
* Professional developer since 1997
* Instructor at Lighthouse Labs and freelance developer

## Why?

The web was fine, then we broke it.

### In the olden days...

1. Click links
2. URL changes
3. Back goes back

### Today

Modern frameworks practically rewrite most of the browser functionality in Javascript:

* It's a single page application!
* Wait, The back button doesn't work!
* No problem, let's add `#anchors` to our URLs and push them to `history`!
* That's janky AF, let's intercept and take over the URL bar! This way we can write our own router with a bunch of URLs that never make a request!
* All is fine and dandy now but WAIT! Google can't find our content!
* No problem, let's use Node to render our client-side components on the server!
* But what about our client-side routes?
* LET'S RUN OUR CLIENT-SIDE ROUTER ON THE SERVER

Facepalm.

Also: have you heard of Chrome's upcoming [`noscript` intervention](https://timkadlec.com/remembers/2018-09-06-chromes-noscript-intervention/)?

## To be clear...

I'm not talking about apps! The problem is everyone is hellbent in solving everything with an app - including content distribution.

Modern Javascript frameworks are NOT good at that. But you know what's good?

Old fashioned request-response!

## But people want an app-like experience!

No.

People want to read your listicle, see some gifs and be able to share your content easily. That includes searching for it!

## But Google uses chrome-headless to index websites! Javascript is a first-class citizen of the internet now!

Google isn't a monopoly (yet). 

Privacy-conscious people prefer alternatives like DuckDuckGo.

macOS shipped with DDG as default, but it's now... Bing!

## But I don't want my site to be boring!

CSS can take care of 99% of the excitement you need.

The rest can be added with a bit of JS, but always using progressive enhancement (i.e., ideally it should also work without JS).

## This sounds oldschool. Do you want us to use jQuery?

jQuery is not needed anymore.

Use plain vanilla JS when necessary.

If you need to create components, try lightweight solutions like StimulusJS or VueJS.

https://stimulusjs.org/
https://vuejs.org/v2/guide/#Getting-Started

Vue was built to play nice with existing request-response websites. 

It's **much** lighter than React and works very well without a compilation step, so it can be included only where necessary.

React, on the other hand, really wants to be the only thing controlling the DOM, which makes it the worst option to progressively enhance content outlets. 

