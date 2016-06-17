---
id: 107
title: About Me
date: 2013-12-17T07:12:17+00:00
author: Mindy Huang
layout: page
comments: false
tags: [about]
---

A picture is worth a thousand words, so here's a 10000 word article.

{% capture images-build %}
    http://i416.photobucket.com/albums/pp249/KCHuang/Blog/10818405_10152806594358435_6207630468232748854_o.jpg
    http://i416.photobucket.com/albums/pp249/KCHuang/Blog/10306772_10152556639780572_2778534272439400781_n.jpg
{% endcapture %}

{% include gallery images=images-build cols=2 %}

{% capture images-art %}
	http://i416.photobucket.com/albums/pp249/KCHuang/Blog/13244886_1399738160039967_9008844896564659491_n.jpg
	http://i416.photobucket.com/albums/pp249/KCHuang/Blog/12496499_10205446572954663_4635184459792717522_o.jpg
{% endcapture %}
{% capture images-art2 %}
	http://i416.photobucket.com/albums/pp249/KCHuang/Blog/12633586_10205169643831608_4166273206412816688_o.jpg
{% endcapture %}
{% include gallery images=images-art cols=2 %}
{% include gallery images=images-art2 cols=1 %}

Actually I'm not a very contentious person. But it rhymed and I appreciate that :)

{% capture images-fight %}
	http://i416.photobucket.com/albums/pp249/KCHuang/Blog/fourth_kyu_cover-1038x576.jpg
	http://i416.photobucket.com/albums/pp249/KCHuang/Blog/12983797_10153954197516539_6553184980669688243_o.jpg
{% endcapture %}
{% include gallery images=images-fight cols=1 %}
<!-- {% include gallery images=images-fight caption="Aikido, Eskrima. I've also done a small amount of jiujutsu, TKD, BJJ, and Parkour. Always excited to learn more." cols=1 %} -->

<img src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/stanford_engineering.png" />
