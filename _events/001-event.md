---
layout: splash
$paragraph-indent: true
permalink: /events/001-event/
date: 2018-06-01
title: 'Waseda University Lectures'
url_: 
pdf_url: 
sub: 1
type: 
links:
  - sub_title: 'Lecture 1: Multilinear Algebra and Tensor Decompositions.'
    url: 
    pdf_url: /assets/events/Lesson 1 Multilinear Algebra and Tensor Decompositions.pdf
  - sub_title: 'Lecture 2: Tensor Networks.'
    url: 
    pdf_url: /assets/events/Lesson 2 tensor networks.pdf
  - sub_title: 'Lecture 3: Tensor Methods for Signal Processing and Machine Learning.'
    url: 
    pdf_url: /assets/events/Lesson 3 Tensor Methods for Signal Processing and Machine Learning.pdf
---



<link rel="stylesheet" href="/assets/css/bootstrap.css">

<style>

  .entry-headers {
    padding-top: 1.0em;
  }

.page__footer-follow li {
  display: inline-block;
  padding-top: 5px;
  padding-bottom: 20px;
  font-size: .8em;
  text-transform: none;
}

td {
    border-bottom: 1px solid #fff;
}

a {
    color: #158CBA;
}

#gridid i {
    font-size: 16px;
    font-style: italic;
}


li {
    font-size: 12px;
}

.paper-btn {
    background-color: #158CBA;
    border: none;
    color: white;
    padding: 2px 2px;
    font-size: 12px;
    cursor: pointer;
    border-radius: 15%;
}


.news-date {
    font-size:1.0em;
    color:#5481B0;
  }
  .news-title {
    font-size:0.8em;
  }

  .news-p p {
    font-size:1.0em;
    margin-bottom: 1.0em;
    text-align: start; 
  }

  .news-a a {
    font-size:1.0em;
    color: #158CBA;
  }

</style>
<div style="padding-bottom: 20rem;" class="container-home page__other__hero--overlay">
  <h1 style="text-transform: capitalize" class="entry-headers"> events </h1>
  <br><br>
  <div class="news-a">
    <section class="news-p">
      <span class="news-date"><b>{{ page.date | date: "%b %Y" }}</b></span><br>
      {% if page.url.size > 0 %}
      <a href="{{ page.url | default: '#' }}"><button class="paper-btn"><i style="font-style:normal" class="fa fa-link"></i>&nbsp;Website</button></a>
      {% endif %}
      {% if page.pdf_url.size > 0 %}
      <a href="{{ page.pdf_url | default: '#' }}"><button class="paper-btn"><i style="font-style:normal" class="fa fa-book"></i>&emsp;&nbsp;PDF&emsp;</button></a>
      {% endif %}
      &nbsp;<b>{{ page.title }}</b>&nbsp;
      <br>
      {% if page.sub == 1 %}
        {% for link in page.links %}
        &emsp;&emsp;
        {% if link.url.size > 0 %}
        <a href="{{ link.url | default: '#' }}"><button class="paper-btn"><i style="font-style:normal" class="fa fa-link"></i>&nbsp;Website</button></a>
        {% endif %}
        {% if link.pdf_url.size > 0 %}
        <a href="{{ link.pdf_url | default: '#' }}"><button class="paper-btn"><i style="font-style:normal" class="fa fa-book"></i>&nbsp;PDF</button></a>
        {% endif %}
        {{ link.sub_title }}
        <br>
        {% endfor %}
      {% endif %}
    </section>
    <br>
    <hr>
  </div> 
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
                <li>
                  <strong>Contact Info:</strong><br>Email: qibin.zhao [at] riken.jp &nbsp;*Please replace "[at]" with "@"<br>Tel: +81-(0)3-6225-2539<br><strong>Follow:</strong>
                  <!-- &nbsp;<a href="https://github.com/" rel="nofollow noopener noreferrer"><i style="font-style:normal"  class="fab fa-fw fa-github-square" aria-hidden="true"></i> GitHub</a>&nbsp;&nbsp; -->
                  &nbsp;<a href="https://twitter.com/rikenaiptlt" rel="nofollow noopener noreferrer"><i style="font-style:normal" class="fab fa-fw fa-twitter-square" aria-hidden="true"></i> Twitter</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="page__footer-copyright" style="padding-left: 30px; padding-right: 30px; color:#808080">© 2023 Tensor Learning Team. Powered by <a href="https://jekyllrb.com" rel="nofollow">Jekyll</a>.
          </div>
        </div>
      </div>
    </div>
