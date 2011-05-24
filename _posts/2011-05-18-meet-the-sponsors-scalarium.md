---
layout: post
title: Meet the sponsors: scalarium
---

[Scalarium.com](http://www.scalarium.com) is one of the main sponsors of EuRuKo 2011 and we would like to talk a bit about what we do.

It all started with the guys at Peritor working hard on consulting gigs and helping people move their applications to Amazon EC2. Doing this is complex and involves a lot of repetition. Also Amazon EC2 lacks some fundamental capabilities like automatic replacement of dead hosts, easy configuration, or application deployment support.
So Scalarium was born to fill that gap. Running in production for over a year now, Scalarium now hosts some pretty big and popular sites. Scalarium is a management layer on top of EC2 that automates the hell out your machines and gives you:

 * Configuration with Chef
 * Auto healing and replacement of failed hosts
 * Auto scaling by time of day or load on your machines
 * Build-in deployment and logging
 * Extensive monitoring and tracking
 
The most important component of Scalarium is the local agent running on every machine. It communicates the local state up to the main repository and responds to changes by executing Chef runs. Scalarium uses Chef to form servers into your desired state. What differentiates Scalarium from a simple Chef server setup is that Scalarium generates life-cycle events (like setup, deployment or state change) and pushes them down to all machines rather then relying on Chef server pull. By having multiple life-cycle events you can tell Scalarium what to do when servers come or go or how to respond to a new application server (e.g. by adding it to the load balancer!). Also Scalarium takes care of EC2, abstracting the API & co away.
You model your architecture by using build-in roles (like Rails app server, MySQL server, load balancer or Node.js app server) or by creating custom definitions. Thanks to the power of Chef, Scalarium can automate anything scriptable.

![scalarium_overview](/images/scalarium_overview.png)

Using the provided auto scaling mechanisms many clients scale down machines during the night and boot them over the day. This saves a lot of money as you only pay for what you are actually using.

Our team is based in Berlin and apparently trusted so much that we are the save-keeper of the EuRuKo gong.

![scalarium_office](/images/scalarium_office.png)

We work with Rails, Nanite, AMQP, RabbitMQ, CouchDB, Redis, and Chef and spend our time hacking Ruby backend code, writing Chef recipes for exciting new tech like Node.js or complaining about various Linux distros. Oh, and we are migrating our frontend to Backbone.js too. If you are a Ruby developer or a Linux sysadmin looking for a job maintaining hundreds of servers, drop us a line at <jobs@scalarium.com>.