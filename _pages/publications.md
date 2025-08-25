---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
---

<style>
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
### Preprints
{% bibliography --query @unpublished %}
</div>

<div class="jumbotron">
### Conference Papers
{% bibliography --query @inproceedings %}
</div>


<div class="jumbotron">
### Journal Articles
{% bibliography --query @article %}
</div>


<div class="jumbotron">
### Tools
{% bibliography --query @software%}
</div>

<div class="jumbotron">
### PhD Thesis
{% bibliography --query @phdthesis%}
</div>

<div class="jumbotron">
### Masters Thesis
{% bibliography --query @mastersthesis%}
</div>

