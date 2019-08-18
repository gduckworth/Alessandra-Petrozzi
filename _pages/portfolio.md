---
layout: archive
title: "Gallery"
permalink: /portfolio/
author_profile: false
sidebar:
  nav: "sidenav"
---

<div class="grid__wrapper">

<script type="text/javascript" src="path/to/instafeed.min.js"></script>

<div id="instafeed"></div>

var feed = new Instafeed({
            get: 'user',
            userId: '16651177378',
            template: '<a href="{{link}}"><img class="insta-image" src="{{image}}" /></a>',
            accessToken: 'bfd5aafc0a674124a18ba1caecd02300'
        });
        feed.run();


<script src="jquery.instagramFeed.min.js"></script>
<script>
    (function($){
        $(window).on('load', function(){
            $.instagramFeed({
                'username': 'bertdumbo',
                'container': "#instagram-feed1",
                'display_profile': true,
                'display_biography': true,
                'display_gallery': true,
                'callback': null,
                'styling': true,
                'items': 8,
                'items_per_row': 4,
                'margin': 1 
            });
        });
    })(jQuery);
</script>


<script src="jquery.instagramFeed.min.js"></script>
<script>
    (function($){
        $(window).on('load', function(){
            $.instagramFeed({
                'username': '16651177378',
                'container': "#instagram-feed1",
                'display_profile': true,
                'display_biography': true,
                'display_gallery': true,
                'callback': null,
                'styling': true,
                'items': 8,
                'items_per_row': 4,
                'margin': 1 
            });
        });
    })(jQuery);
</script>


<p>Please be aware this page is currently under construction and should be available in the near future.</p>  
  {% for post in site.podcast %}
    {% include archive-single.html type="grid" %}
  {% endfor %} 
</div>
