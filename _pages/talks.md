---
title: "Talks"
layout: gridlay
sitemap: false
permalink: /talks/
---

<style>
.btn{
    margin-bottom:5px;
    padding-top:1px;
    padding-bottom:1px;
    padding-left:15px;
    padding-right:15px;
}
.jumbotron{
    padding:3%;
    padding-bottom:10px;
    padding-top:10px;
    margin-top:10px;
    margin-bottom:30px;
    width: calc(100% + 60px);
    margin-left: -30px;
    margin-right: -30px;
    max-width: none;
}
</style>

<div class="jumbotron">
### Talks
<ol class="bibliography" reversed="reversed">
{% for t in site.data.talks %}
    <li>
        <div class="text-justify">
            <div class="paper-entry">
                <div class="paper-title">{{ t.title }}{% if t.keywords contains "invited" %} (invited){% endif %}</div>
                <div class="paper-venue">at {% if t.venueurl %}<a href="{{ t.venueurl }}" target="_blank" rel="noopener noreferrer">{{ t.publisher }}</a>{% else %}{{ t.publisher }}{% endif %}</div>
            </div>
        </div>

        {% if t.video %}<a href="/talks/{{ t.video }}" target="_blank"><button class="btn btn-emerald btm-sm">Video</button></a>{% endif %}
        {% if t.slides %}<a href="/slides/{{ t.slides }}" target="_blank"><button class="btn btn-amber btm-sm">Slides</button></a>{% endif %}
    </li>
{% endfor %}
</ol>
</div>

