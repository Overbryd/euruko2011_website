---
layout: default
title: Agenda – EuRuKo 2011
javascripts:
  - "http://code.jquery.com/jquery-1.6.min.js"
  - "fancybox/jquery.fancybox-1.3.4.pack.js"
stylesheets:
  - "fancybox/jquery.fancybox-1.3.4.css"
---

<script type="text/javascript">
  $(function() {
    var $body = $('<div></div>').hide().appendTo($('body'));
    
    $.get('/visitor_info.html', function(data) {
      $(data).find('#visitor-info-map').appendTo($body);
      
      $('a:contains(Visitor Info Map)')
        .attr('href', '#visitor-info-map')
        .fancybox({
          'transitionIn': 'elastic',
          'transitionOut': 'elastic',
          'speedIn': 150, 
          'speedOut': 100, 
          'overlayShow': false,
          'hideOnContentClick': true
        });
    });
    
    $.get('/speakers.html', function(data) {
      $(data).find('#speakers li').each(function() {
        var $this = $(this),
          name = $this.find('h3').text(),
          domID = $this.find('a:first').attr('name'), //name.toLocaleLowerCase().replace(/[^a-z]/u, '-'),
          $div = $('<div></div>'),
          $link = $('<a></a>'),
          $toggle = $('.schedule td:contains('+name+')');
                
        $div
          .attr({ 'class' : 'speaker', id : domID })
          .html($this.html())
          .appendTo($body);
        
        $link
          .text($toggle.text())
          .addClass('speaker-link')
          .attr('href', '#'+domID)
          .fancybox({
            'transitionIn': 'elastic',
            'transitionOut': 'elastic',
            'speedIn': 150, 
            'speedOut': 100, 
            'overlayShow': false,
            'hideOnContentClick': true
          });
        
        $toggle.html($link);
      });
      // $(window.document).trigger('euruko:speakers-loaded');
    });
  });
</script>

## Friday

<h3>&nbsp;</h3>
### Pre Conference Meetup

![c-base logo](/images/c-base-logo.png)  
All people who arrive on friday are invited to the pre conference meetup at [c-base](http://www.c-base.org/).  
The c-base is an awesome space ship landed in Berlin. We start around 21:00.

You can find it on our [Visitor Info Map](http://goo.gl/maps/gwcZ). The closest subway/S-Bahn station is called "S+U Jannowitzbrücke". 

## Saturday

### Schedule

<table class="schedule">
  <thead>
    <tr>
      <th>Time</th>
      <th>What</th>
      <th>Speaker</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>09:00</td>
      <td colspan="2">Registration</td>
    </tr>
    <tr>
      <td>09:30</td>
      <td colspan="2">Welcome</td>
    </tr>
    <tr>
      <td>09:45</td>
      <td>Keynote</td>
      <td>Yukihiro Matsumoto</td>
    </tr>
    <tr class="pause">
      <td>10:45</td>
      <td colspan="2">Coffee Break</td>
    </tr>
    <tr>
      <td>11:00</td>
      <td>Ruby helps us make movies: Guerilla-DI, scripted tools for a modern film pipeline</td>
      <td>Julik Tarkhanov</td>
    </tr>
    <tr>
      <td>11:30</td>
      <td>JRuby hacking guide</td>
      <td>David Calavera</td>
    </tr>
    <tr>
      <td>12:00</td>
      <td>In the Loop</td>
      <td>Lourens Naudé</td>
    </tr>
    <tr class="pause">
      <td>12:30</td>
      <td colspan="2">Lunch</td>
    </tr>
    <tr>
      <td>14:30</td>
      <td>Games for the Masses: Scaling Rails to the Extreme</td>
      <td>Jesper Richter-Reichhelm</td>
    </tr>
    <tr>
      <td>15:00</td>
      <td>BE RESTFUL. BE WEB 2.0. BUT DON'T MIX IT</td>
      <td>Nick Sutterer</td>
    </tr>
    <tr>
      <td>15:30</td>
      <td>Actors on Stage</td>
      <td>Elise Huard</td>
    </tr>
    <tr class="pause">
      <td>16:00</td>
      <td colspan="2">Longer Break</td>
    </tr>
    <tr>
      <td>16:30</td>
      <td>The Expression Problem in Ruby: A focus on Traits.</td>
      <td>Federico Brubacher</td>
    </tr>
    <tr>
      <td>17:00</td>
      <td>The Revenge of method_missing()</td>
      <td>Paolo Perrotta</td>
    </tr>
    <tr>
      <td>17:30</td>
      <td>Lightning Talks</td>
    </tr>
    <tr class="pause">
      <td>18:30</td>
      <td colspan="2">Dinner Time</td>
    </tr>
  </tbody>
</table>

### Party

![Tante Käthe Logo](/images/tante-kaethe-logo.png)  
We invite you to party with us and all the EuRuCamp visitors at "Tante Käthe" (aka. "Mauersegler"). This location is a pretty unknown jewel of Berlin located right inside the Mauerpark. As hard as it is to find ([Street View](http://maps.google.de/maps?f=q&source=s_q&hl=de&geocode=&q=mauerpark+berlin&aq=&sll=51.151786,10.415039&sspn=16.735226,33.310547&ie=UTF8&hq=mauerpark&hnear=Berlin&ll=52.540371,13.403385&spn=0.007909,0.016265&z=16&layer=c&cbll=52.540408,13.403523&panoid=v3hyRH1ZE4cC4leMB2qyjw&cbp=12,314.38,,0,0.79)), as fun it will get. There's a barbecue waiting for you, lots of beers and a relaxed atmosphere.

Getting to the location might be a bit hard. We try to make it easy for you, by providing the possible routes on our [Visitor Info Map](http://goo.gl/maps/oU1Y). We will also provide flyers with exact directions.

# Sunday

### Schedule
<script type="text/javascript">
  $('.schedule ')
</script>
<table class="schedule">
  <thead>
    <tr>
      <th>Time</th>
      <th>What</th>
      <th>Speaker</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>10:00</td>
      <td>Keynote</td>
      <td>Paul Campbell</td>
    </tr>
    <tr class="pause">
      <td>11:00</td>
      <td colspan="2">Coffee Break</td>
    </tr>
    <tr>
      <td>11:15</td>
      <td>Bridging the gap - Using JavaScript in Rails to write DRY rich client applications</td>
      <td>Thorben Schröder / Andreas Haller</td>
    </tr>
    <tr>
      <td>11:45</td>
      <td>Scanning Strings at Supersonic Speed</td>
      <td>Kornelius Kalnbach</td>
    </tr>
    <tr>
      <td>12:15</td>
      <td>Your Data, Your Search</td>
      <td>Karel Minařík</td>
    </tr>
    <tr class="pause">
      <td>12:45</td>
      <td colspan="2">Lunch</td>
    </tr>
    <tr>
      <td>14:45</td>
      <td>Tales of the Big White Cloud</td>
      <td>Pat Allan</td>
    </tr>
    <tr>
      <td>15:15</td>
      <td>Endless fun with Arduino and Eventmachine</td>
      <td>Bodo Tasche</td>
    </tr>
    <tr>
      <td>15:45</td>
      <td>Getting Hands On with Adhearsion</td>
      <td>Ben Klang / Ben Langfeld</td>
    </tr>
    <tr class="pause">
      <td>16:15</td>
      <td colspan="2">Longer Break</td>
    </tr>
    <tr>
      <td>16:45</td>
      <td>sentiment analysis of Twitter messages in Ruby</td>
      <td>Mateusz Drożdżyński</td>
    </tr>
    <tr>
      <td>17:15</td>
      <td>Writing your own programming language to understand Ruby better</td>
      <td>José Valim</td>
    </tr>
    <tr>
      <td>17:45</td>
      <td colspan="2">Short Lightning Talks</td>
    </tr>
    <tr>
      <td>18:15</td>
      <td colspan="2">Closing, candidates discussion for hosting Euruko 2012</td>
    </tr>
    <tr class="pause">
      <td>18:30</td>
      <td colspan="2">Dinner Time</td>
    </tr>
  </tbody>
</table>
