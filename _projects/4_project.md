---
layout: page
title: Project with comment
description: a project without thumbnail, without category
img: 
importance: 2
category: fun
comments: true
---

***

## content of the project

abcde

> - no category line will make the project not appear
> - category blank would have no appearance
> - only category fun and work accepted

## try making comment appear with the block of liquid code

This is the safe way

> - select the block of code inside the liquid tags

However, try going the standard route is better

> - edit the html layout and copy the universal code provided by disqus
> - right now the code do not work for this project. There is comment in the 1st project loaded for the new disqus shortname only
> - use code provided my al-folio make it work. The difference lie in the disqus_shortname and identifier.

## try making icon appear with link to specific site

> - find the liquid code in the about layout
> - `_pages/about.md` state that social tags is true, investigate `_layouts/about.html`
> - `_includes/social.html` seem like the place that print the social icon code
> - print github icon with link inside the social class html to make it appear in the center
> - can link the github icon appearance to front matter to automate the process

***

<div class="social">
  <div class="contact-icons">
    <a href="https://github.com/thehung92/treemixTools" title="GitHub"><i class="fab fa-github"></i></a>
  </div>
</div>


***

<!-- 
<div id="disqus_thread"></div>
<script type="text/javascript">
      var disqus_shortname  = '{{ site.disqus_shortname }}';
      var disqus_identifier = '{{ page.id }}';
      var disqus_title      = {{ page.title | jsonify }};
      (function() {
        var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
        dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
        (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
      })();
    </script>
<noscript>Please enable JavaScript to view the <a href="http://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
-->