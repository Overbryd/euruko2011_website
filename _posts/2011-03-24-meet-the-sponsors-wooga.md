---
layout: post
title: "Meet the Sponsors: wooga"
---

[wooga](http://www.wooga.com) is one of the main sponsors for the conference this year, and to introduce the company,
Tim Lossen (one of the organizers of the conference and a lead engineer at wooga) sat down to
talk about the [working atmosphere in wooga’s Berlin HQ](http://www.wooga.com/jobs/office-tour/) and his experiences with using Ruby with
social games.

First of all, Tim specifically works on one of wooga’s games, “[Happy Hospital](http://www.facebook.com/campaign/landing.php?campaign_id=153492964705221&partner_id=wooga&placement=7&url=http://www.facebook.com/HappyHospital)”. He is part of a
cross-functional team that consists of product managers, designers, flash developers, and
backend developers &mdash; twelve people in total. He is responsible not only for developing new game
features, but also keeping everything running smoothly 24/7 &mdash; in short, you could say he’s
responsible for devops.

The setup is as follows: the backend is a rails app, running on a small cluster with a fairly
standard configuration: haproxy as the load balancer, nginx as the web server and unicorn for
the app server. The interesting part is that the team decided early on to ditch MySQL and use
Redis as the main database. According to Tim, “that decision was awesome for performance, but
brings some unique challenges as well.” One of the primary languages in use is of course Ruby,
because “game development is always moving pretty quickly. We do weekly iterations, so we need a
language that doesn’t stand in our way. When you’re working with a small team and a short time
frame, you want your language to work with you, not against you”. Some people might say that
Ruby is too slow for this setup &mdash; but while Ruby is indeed slow, that has never proven to be a
problem for the team.

![work desk](/images/sponsors/wooga1.jpg)
He even has a window, with twice the legal minimum space required by German law for a 
<strike>farm animal</strike> beloved programmer!

But what is really awesome about working at wooga isn’t necessarily the setup the team gets to
work with &mdash; but rather that they got to choose exactly how they wanted to set everything up. No
one on the [Happy Hospital](http://www.facebook.com/campaign/landing.php?campaign_id=153492964705221&partner_id=wooga&placement=7&url=http://www.facebook.com/HappyHospital) team has ever felt like they were being micro-managed and forced down
a specific path &mdash; which is great, because the last thing any programmer wants is to have a
non-technical person breathing down their necks, telling them what to do. But with this kind of
freedom comes a great deal of responsibility. The [Happy Hospital](http://www.facebook.com/campaign/landing.php?campaign_id=153492964705221&partner_id=wooga&placement=7&url=http://www.facebook.com/HappyHospital) team knows that they are
responsible for making sure their decisions actually work, and that they can carry out the
choices they have made.

Each game at wooga is started off as a greenfield development. This means that the people who
best know what they’re doing have the freedom to make a lot of the technical decisions &mdash;
from selecting the programming language, framework and database, to choosing the hosting 
provider &mdash; and as long as they can reasonably justify their choices, there is no 
pressure to conform to a preset path.

The last thing Tim talked about, is that the most challenging part of building social games is
the sheer size of everything. Everyone involved in creating a game needs to keep in mind that
you need hundreds of thousands of daily active users in order to produce a successful game on
Facebook, and this leads to some very interesting scaling issues on the technical side. What
works in the office is radically different from what works in the wild, and Tim says that this
is definitely one of the most interesting parts of his job.

![super secret game concepts](/images/sponsors/wooga2.jpg)
Super secret game concepts, in our creative room &mdash; please do not distribute ...

If you come to Berlin and fall in love with the city, [apply](http://www.wooga.com/jobs/) and you’re more than welcome to
stay! But before you make up your mind, read about how we are one of the few start ups
[challenging Silicon Valleys dominance](http://eu.techcrunch.com/2011/03/17/europes-wooga-moves-up-the-social-gaming-leader-board-but-silicon-valley-dominates/)
or about [our latest game](http://www.wooga.com/2011/03/diamonddash/). We have an incredibly creative,
free flowing office and a team of highly skilled people from all over the world.

### About wooga

Based in Berlin, wooga (world of gaming) is Europe’s largest social game developer. Founded in
2009, the company has quickly grown to over 70 employees from 20 different countries. With more
than 18 million active users per month, wooga is the fifth largest social gaming company in the
world. Wooga focuses on producing high quality games for Facebook, with an emphasis on
compelling characters, ease of use and professional localization in seven languages. 
[Diamond Dash](http://www.wooga.com/games/diamonddash/) is wooga’s fifth game, 
preceded by [Brain Buddies](http://www.wooga.com/games/brain-buddies/), 
[Bubble Island](http://www.wooga.com/games/bubble-island/), 
[Monster World](http://www.wooga.com/games/monster-world/) 
and [Happy Hospital](http://www.wooga.com/games/happy-hospital/).


