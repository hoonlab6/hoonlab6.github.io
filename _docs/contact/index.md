---
layout: page
title: "Contact"

---


<link href="https://fonts.googleapis.com/css2?family=Noto+Sans:wght@700&display=swap" rel="stylesheet">
<style>
body {
    font-family: 'Noto Sans', sans-serif; font-size: 22px;
}
</style>


<i class="fa fa-twitter"></i> Follow <a href="https://twitter.com/wisekh6" title="Follow @wisekh6" alt="Follow @wisekh6">@wisekh6</a> for lab updates and information related to our research.

## Correspondence

Hoon Kim, PhD  

Associate Professor  
Biomedical Convergence    
Dept. of Pharmacy    
Sungkyunkwan Univ        
Seobu-ro, Jangan-gu, Suwon-si    
Gyeonggi-do, South Korea, 16419


<i class="fa fa-phone"></i> +1-212-444-8121  
<i class="fa fa-paper-plane"></i> <wisekh6@gmail.com>  
<i class="fa fa-twitter"></i> <a href="https://twitter.com/intent/tweet?via={{ site.owner.twitter }}&amp;hashtags=website" target="_blank" title="Tweet Hoon Kim">Tweet Hoon Kim</a>  

## Administrative Support

Available soon

<i class="fa fa-phone"></i> +82-
<i class="fa fa-paper-plane"></i> `<first_name>.<last_name>` at skku.kr.edu


<!-- Open Positions, if any, will populate here -->

<div class="row">
<div id="accordion col-sm-12"><hr class="small"></div>
<div id="accordion col-sm-12">
<div id="accordion">
  {% assign counter = 1 %}
  {% for post in site.categories.positions limit:5 %}
  {% if post.postjob == true %}
  <h4><i class="iconfont"></i> {% if post.date %}<time class="icon-calendar pr20" datetime="{{ post.date | date: "%Y-%m-%d" }}" itemprop="datePublished"> {{ post.date | date: "%Y-%m-%d" }}</time> {% endif %}{{ post.title }}</h4>
    <div>
      {% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% elsif post.teaser %}{{ post.teaser | strip_html | escape }}{% elsif post.excerpt %}{{ post.excerpt | markdownify | remove: '<p>' | remove: '</p>' }}{% endif %}
      <a href="{{ site.url }}{{ post.url }}" title="Read {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a>
    </div>
  {% endif %}
  {% assign counter=counter | plus:1 %}
  {% endfor %}
</div></div>
</div>


<script>
$(function() {
  $( "#accordion" ).accordion({
      heightStyle: "content"
  });
});
</script>


