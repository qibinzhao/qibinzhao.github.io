---
layout: splash
$paragraph-indent: true
permalink: /news/004-news/
title: 'Our paper has been accepted to ICLR 2018 (Workshop).'
date: 2018-01-01
news_content: ''
number_photo: 0
photo1: 
photo2: 
---



<link rel="stylesheet" href="/assets/css/bootstrap.css">

<style>
  img{
      max-width:345px;
      max-height:258px;
      OBJECT-FIT:contain;
  }


.entry-headers {
  padding-top: 1.0em;
}

#gridid i {
    font-size: 16px;
    font-style: italic;
}

.page__footer-follow li {
  display: inline-block;
  padding-top: 5px;
  padding-bottom: 20px;
  font-size: .8em;
  text-transform: none;
}

.news-date {
  font-size:1.0em;
  color:#5481B0;
}
.news-title {
  font-size:1.0em;
}

.news-p p {
  font-size:1.1em;
}

.news-a a {
  font-size:1.0em;
  color: #158CBA;
}
</style>

<div style="padding-bottom: 20rem;" class="container-home page__other__hero--overlay">
  <h1 style="text-transform: capitalize" class="entry-headers"> News </h1>
  <br>
  <div class="news-a">
    <section class="news-p">
      <span class="news-date"><b>{{ page.date | date: "%b %Y" }}</b></span>
      <br>
      <b>{{ page.title }}</b>
      <p>&emsp;{{ page.news_content }}</p>
      {% if page.number_photo == 1 %}
      <div class="row">
        <div class="col-sm-12">
          <img src="/assets/images/news/{{ page.photo1 }}" class="img-responsive" width="100%">
        </div>
      </div>
      {% endif %}
      {% if page.number_photo == 2 %}
      <div class="row">
        <div class="col-sm-6 clearfix">
          <img src="/assets/images/news/{{ page.photo1 }}" class="img-responsive" width="100%">
        </div>
        <div class="col-sm-6 clearfix">
          <img src="/assets/images/news/{{ page.photo2 }}" class="img-responsive" width="100%">
        </div>
      </div>
      {% endif %}
    </section>
  </div>
  <br><br><br><br><br><br><br>
</div>

<div style="position: absolute; bottom: 0;" class="page__footer">
  <footer-new>
    <div class="row">
      <div id="gridid" class="col-sm-12">
        <div class="row">
          <div class="col-sm-6 clearfix" style="padding-left: 30px; padding-right: 30px">
            <div class="page__footer-follow">
              <ul class="social-icons">
                <li><strong>Access:</strong><br>Nihonbashi 1-chome Mitsui Building, 15th floor,<br>1-4-1 Nihonbashi,Chuo-ku, Tokyo<br>103-0027, Japan &nbsp; <a href="https://goo.gl/maps/KfJb19p3ZQLqYjae7" rel="nofollow noopener noreferrer">（<i style="font-style:normal" class="fa fa-location-arrow" aria-hidden="true"></i> Map） </a></li>
              </ul>
            </div>
          </div>
          <div class="col-sm-6 clearfix" style="padding-left: 30px; padding-right: 30px">
          <!-- start custom footer snippets -->
          <!-- end custom footer snippets -->
            <div class="page__footer-follow">
              <ul class="social-icons">
                <li><strong>Contact Info:</strong><br>Email: qibin.zhao [at] riken.jp &nbsp;*Please replace "[at]" with "@"<br>Tel: +81-(0)3-6225-2539<br><strong>Follow:</strong>&nbsp;<a href="https://github.com/" rel="nofollow noopener noreferrer"><i style="font-style:normal" class="fab fa-fw fa-github-square" aria-hidden="true"></i> GitHub</a>&nbsp;&nbsp;&nbsp;<a href="https://twitter.com/rikenaiptlt" rel="nofollow noopener noreferrer"><i style="font-style:normal" class="fab fa-fw fa-twitter-square" aria-hidden="true"></i> Twitter</a></li>
              </ul>
            </div>
          </div>
          <div class="page__footer-copyright" style="padding-left: 30px; padding-right: 30px; color:#808080">© 2023 Tensor Learning Team. Powered by <a href="https://jekyllrb.com" rel="nofollow">Jekyll</a>.
          </div>
        </div>
      </div>
    </div>
