---
layout: archive
title: "Portfolio"
permalink: /portfolio/
author_profile: false
sidebar:
  nav: "sidenav"
---

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
