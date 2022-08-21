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
}
</style>

<!-- <div class="jumbotron">
### Preprints
{% bibliography --query @unpublished %}
</div>
 -->
<div class="jumbotron">
### Conference proceedings
{% bibliography --query @inproceedings %}
</div>


<div class="jumbotron">
### Journal articles
{% bibliography --query @article %}
</div>


<div class="jumbotron">
### Tools
{% bibliography --query @software%}
</div>

<div class="jumbotron">
### Thesis
{% bibliography --query @thesis%}
</div>

