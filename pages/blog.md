---
layout: page
title: "Blog"
permalink: "/blog"
description: "The blog of hullCSS, the Computer Science at the University of Hull, looking to make the lives of students more exciting and expand technology beyond the course."
---

<span class="bigtext-slogan-thing">Blog</span>
<br><br>

<div class="grid-containter">

{% for post in site.posts %}

<a href="{{post.url}}">
<div class="post-item grid-33 mobile-grid-100">
<div class="image-blog" style="background-image:url('{{site.url}}/images/blog/{{post.image}}')" >
<div class="text-blog-desc">
<div class="text-blog-pad">
<div class="main-text"> {{post.title}}</div>
<br>
<div class="date-text"> {{ post.date | date: "%-d %B %Y" }} </div>
</div>
</div>
</div>
</div>
</a>
{% endfor %}

</div>

<style>
.image-blog {
    height: 300px;
    padding: 25px;
    background-size: cover;
    border-radius: 2%;
        background-position: center;
}

.text-blog-desc {
        background-color: #333;
    padding: 10px 20px;
    border-radius: 5px;
    opacity: 0.8;
    margin-top: 150px;
}

.main-text {
    font-size: 18px;
    font-family: 'roboto mono';
    margin-bottom: -10px;
    text-align: center;
}

.date-text {
    text-align: center;
    font-weight: 400;
    font-family: 'roboto';

}


</style>
