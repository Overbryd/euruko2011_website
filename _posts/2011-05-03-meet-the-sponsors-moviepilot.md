---
layout: post
title: "Meet the Sponsors: moviepilot"
---

Hey there, my name is [Jannis](http://moviepilot.de/users/jannis) and I’m responsible for things like coffee and recommender systems at [moviepilot.de](http://moviepilot.de) and I’d like to tell you something about us.

In 2007 two guys, let’s call them [Tobi](http://www.moviepilot.de/users/tobias) and [Jon](http://www.moviepilot.de/users/jonni), decided to leave the movie production game and start an online movie community. Moviepilot is a fast growing European movie community with an innovative social utility - offering the first completely personalized entertainment guide in Europe. We provide detailed information to more than 50,000 movies to which we are able to deliver individual predictions on how the user will like a movie. 

Upon registration, each user creates a short taste profile by quickly rating a few films. We then look for those users whose tastes in movies are most alike and are able to give individual predictions for movies and make recommendations that pay off. By now we have over 100,000 registered users, 120,000 celebrities and more than 10 mio. film ratings in the database which makes us Germany's largest film-community.

![Writing on windows](http://dl.dropbox.com/u/1953503/euruko/euruko1.jpg)

_Like well known [Beautiful Mind](http://www.moviepilot.de/movies/a-beautiful-mind-genie-und-wahnsinn)s, we like to draw on things._

But all this started out circulating excel sheets amongst the employees to gather info about their taste in movies. Then we got our friends to fill out the questionnaires and tell the moviepilots all about the films they like. The questionnaires were then sent on to friends of friends but we started wondering whether this approach would scale to hundreds of thousands of users. 

The hackers at moviepilot had to figure something out. In 2007 moviepilot’s first recommender engine was born, made with ruby on rails and MySQL. But as the site began to gain traction in 2008, the MySQL based recommender system just didn’t cut the mustard anymore. I was finishing my master’s degree in computer science at that time, and was looking for an interesting place to write my thesis. 

As part of my thesis I built moviepilot’s next generation recommender engine, a custom RESTful webservice that was optimized for performance and integrated into the existing ruby on rails & MySQL infrastructure through background jobs ([resque](http://github.com/defunkt/resque) FTW). The amount of available data still grows every day, and this system allowed us to generate awesome movie recommendations in no time (at some point we actually built a real-time recommender engine).

We quickly realized that in order to make the most out of this never ending well of data we needed <strike>an adult</strike> science. There was no way I could deal with analzying movie recommendations, a huge archive of movie news, and very detailed semantic, emotional, geospatial movie annotations all alone, so we teamed up with the [Technical University of Berlin](http://www.dai-labor.de/irml/forschung/) to do some research together.

![Moviepilots hacking away](http://dl.dropbox.com/u/1953503/euruko/euruko2.jpg)

_Moviepilots hacking away (while browsing moviepilot recommendations on the T-Home set top box in the background)_

In 2009 I went to New York to attend the most important conference in this field, the ACM Recommender Systems Conference (RecSys for short), and it was great. I didn’t want to be passive and just watch other people do cool stuff, though, so in 2010 we held a [full day workshop](http://www.dai-labor.de/camra2010/) about context aware movie recommendations at the RecSys 2010 in Barcelona. We did this together with our great partners at the DAI-Labor of the Technical University in Berlin.

Just last week we received confirmation that our proposal for another full day workshop at the [RecSys 2011](http://recsys.acm.org/2011/index.shtml) in Chicago had been approved. Yay! Also, we’re organizing the Movie Hack Day 2011 in Berlin in June (see <http://moviehackday.com>) so why don’t you come join us?

[![Movie Hack Day Poster](http://dl.dropbox.com/u/1953503/Movie%20Hackday/movie-hackday-berlin-300x458.jpg)](http://moviehackday.com/)

So what’s life at moviepilot like today? The developer team has grown and we’re quite international now, I’m sitting at a big desk with a Swedish data mining expert who is writing his PhD at moviepilot and next to a Catalan graph database guru. Together with Ben, our CTO and Andreas, a fellow developer, I hack away on our new product and at least once a week I meet up with the guys from the DAI-Lab to work on our research project on context aware movie recommendations.

I will be at the conference on the 28th and 29th of May so come and talk to me.

### TL;DR

We love data, science, visualizations and hacking! Come join us, we have open PhD positions with the TU-Berlin and are looking for developers... [mailto:jobs@moviepilot.com](jobs@moviepilot.com)
