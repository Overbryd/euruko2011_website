---
layout: post
title: "Meet the sponsors: SoundCloud"
---
![Souncd Cloud Office](http://www.wechsellook.com/postFiles/25b7acb5-ee99-4616-9eb3-b01718b02118.jpg)

Hey there! My name's Rany and I'm pleased to announce that SoundCloud will be one of the main sponsors of Euruko this year. 

Since its creation in 2007, SoundCloud has run on Rails. We began as a small music sharing platform in private beta, and have grown to become an increasingly essential site for audio sharing on the web with over 4 million users.

Scaling is obviously a big concern. We are not only utilizing proven solutions, but also experimenting with new approaches.

* SoundCloud.com and the API currently run Rails on this stack: Varnish, Nginx, HAProxy, Thin and RabbitMQ
* Assets are served from S3 and we use EC2 for worker tasks.
* We're experimenting with NodeJS and Backbone.js on our [Mobile Site](http://m.soundcloud.com)
* Most of our data is served from MySQL, where we have a classic Master/Slave set-up.
* Cassandra to serve the Dashboards (you can hear Sean talking about that at [Rug_B](http://soundcloud.com/kesselborn/rug-b-cassandra-talks-2011-03)).
* Ruby also comes into play in how we manage our infrastructure. As we continue to grow we'll be adding many new machines. To prepare for this we use Chef for our configuration management.  
* For testing purposes, we use RSpec, Cucumber, and Selenium. Our test suite has grown too large to run locally, so we've decided to run it on Amazon EC2, where we fire up a lot of instances to run the test suite in parallel. Jenkins CI manages our continuous integration of various apps.

Check out some of our experiences on our Backstage blog. For example, here's an amazing post on [how we failed with MongoDB!](http://backstage.soundcloud.com/2011/04/failing-with-mongodb/)


![Souncd Cloud Office](http://www.wechsellook.com/postFiles/f7859c89-bd90-4e43-bae8-31a11218c251.jpg)

We have a strong focus on our API and its developer ecosystem. To assure the quality of our API and its documentation, we actually eat our own dog food: the iOS, Cocoa and Android development happens in-house. We have also launched a shiny, new developer portal making it easier for developers to get started. Our App Gallery, currently showcases over [150 apps](http://soundcloud.com/apps) by external developers.

Currently there are 30 developers running SoundCloud from Berlin. All major development takes place at "Silicon Rosenthaler Platz" in Mitte. Minor development takes place on our rooftop terrace, and we also have satellite offices in San Francisco and London.

![Minor development in action](http://www.wechsellook.com/postFiles/6706584e-3ef1-4f4e-93e5-2bd6254bac45.jpg)

So come say hi and have a beer with us at Euruko! There will be at least four of us Clouders in attendance - Tobi, Sebastian, Daniel, and me. Did I mention that [we're hiring like crazy?](http://soundcloud.com/jobs)

Also, if you were unable to get a ticket to Euruko, we will also be attending [Music Hack Day Berlin] (http://berlin.musichackday.org/2011/) at MTV Networks, to hack on new music apps. Awesome ruby hackers are most welcome! 

