---
title: "Team Members"
layout: splash
excerpt: "Allan Lab: Team members"
sitemap: false
permalink: /members/
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


h4 {
    font-size: 18px;
    display: block;
    margin-block-start: 1.33em;
    margin-block-end: 1.33em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
    font-weight: bold;
}
h4, .h4 {
    margin-top: 12px;
    margin-bottom: 6px;
}

#gridid i {
    font-size: 16px;
    font-style: italic;
}

#gridid ul {
    display: block;
/*    margin-block-start: 5px;
    margin-block-end: 5px;*/
    margin-inline-start: 0px;
    margin-inline-end: 0px;
/*    padding-inline-start: 30px;*/
}

.clearfix li {
    font-size: 12px;
}

.social-icons li {
    font-size: .8em;
}


#gridid img {
    max-height:170px;
    margin: 10px 22px 6px 0;
    border-radius: 10%;
    box-shadow: 2px 2px 5px #888;
}

a {
    color: #158CBA;
}


</style>

<div>
<div id="gridid" style="padding-bottom: 10rem;" class="container-home page__other__hero--overlay">
  <!-- <h1 style="text-transform: capitalize" class="entry-headers"> {{page.title}} </h1> -->
  <br>

  <h2>Team Leader</h2>
  <div class="row">
    {% for member in site.data.team_leader %}
    <div class="col-sm-4 clearfix">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left;"/>
      {% if member.url.size > 0 %}
      <h4><a href="{{ member.url }}">{{ member.name }}</a></h4>
      {% endif %}
      {% if member.url.size == 0 %}
      <h4>{{ member.name }}</h4>
      {% endif %}
      <i style="font-size:90%">{{ member.info }}<br></i>
      {% if member.info2.size > 0 %}
      <a style="color: #696969; font-size:80%">{{ member.info2 }}</a>
      {% endif %}
      <ul style="overflow: hidden; padding-inline-start: 20px;">
        {% if member.number_educ == 1 %}
        <li> {{ member.education1 }} </li>
        {% endif %}
        {% if member.number_educ == 2 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        {% endif %}
        {% if member.number_educ == 3 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        {% endif %}
        {% if member.number_educ == 4 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        {% endif %}
        {% if member.number_educ == 5 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        <li> {{ member.education5 }} </li>
        {% endif %}
      </ul>
    </div>
    {% endfor %}
  </div>

  <h2>Researcher</h2>
  <div class="row">
    {% for member in site.data.researcher %}
    <div class="col-sm-4 clearfix">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left;"/>
      {% if member.url.size > 0 %}
      <h4><a href="{{ member.url }}">{{ member.name }}</a></h4>
      {% endif %}
      {% if member.url.size == 0 %}
      <h4>{{ member.name }}</h4>
      {% endif %}
      <i style="font-size:90%">{{ member.info }} </i>
      <ul style="overflow: hidden; padding-inline-start: 30px;">
        {% if member.number_educ == 1 %}
        <li> {{ member.education1 }} </li>
        {% endif %}
        {% if member.number_educ == 2 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        {% endif %}
        {% if member.number_educ == 3 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        {% endif %}
        {% if member.number_educ == 4 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        {% endif %}
        {% if member.number_educ == 5 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        <li> {{ member.education5 }} </li>
        {% endif %}
      </ul>
    </div>
    {% endfor %}
  </div>
  
  <h2>Student</h2>
  <div class="row">
    {% for member in site.data.student_members %}
    <div class="col-sm-4 clearfix">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" />
      {% if member.url.size > 0 %}
      <h4><a href="{{ member.url }}">{{ member.name }}</a></h4>
      {% endif %}
      {% if member.url.size == 0 %}
      <h4>{{ member.name }}</h4>
      {% endif %}
      <i style="font-size:90%">{{ member.info }} </i>
      <ul style="overflow: hidden; padding-inline-start: 30px;">
        {% if member.number_educ == 1 %}
        <li> {{ member.education1 }} </li>
        {% endif %}
        {% if member.number_educ == 2 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        {% endif %}
        {% if member.number_educ == 3 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        {% endif %}
        {% if member.number_educ == 4 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        {% endif %}
        {% if member.number_educ == 5 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        <li> {{ member.education5 }} </li>
        {% endif %}
      </ul>
    </div>
    {% endfor %}
  </div>


  <h2>Visiting Scientist</h2>
  <div class="row">
  {% for member in site.data.visiting_scientist %}
    <div class="col-sm-4 clearfix">
      <img src="{{ site.url }}{{ site.baseurl }}/assets/images/teampic/{{ member.photo }}" class="img-responsive" width="30%" style="float: left" />
      {% if member.url.size > 0 %}
      <h4><a href="{{ member.url }}">{{ member.name }}</a></h4>
      {% endif %}
      {% if member.url.size == 0 %}
      <h4>{{ member.name }}</h4>
      {% endif %}
      <i style="font-size:90%">{{ member.info }} </i><br>
      {% if member.info2.size > 0 %}
      <a style="color: #696969; font-size:75%">{{ member.info2 }}</a>
      {% endif %}
      <ul style="overflow: hidden; padding-inline-start: 30px;">
        {% if member.number_educ == 1 %}
        <li> {{ member.education1 }} </li>
        {% endif %}
        {% if member.number_educ == 2 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        {% endif %}
        {% if member.number_educ == 3 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        {% endif %}
        {% if member.number_educ == 4 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        {% endif %}
        {% if member.number_educ == 5 %}
        <li> {{ member.education1 }} </li>
        <li> {{ member.education2 }} </li>
        <li> {{ member.education3 }} </li>
        <li> {{ member.education4 }} </li>
        <li> {{ member.education5 }} </li>
        {% endif %}
      </ul>
    </div>
    {% endfor %}
  </div>
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
                <li><strong>Contact Info:</strong><br>Email: qibin.zhao [at] riken.jp &nbsp;*Please replace "[at]" with "@"<br>Tel: +81-(0)3-6225-2539<br><strong>Follow:</strong>&nbsp;<a href="https://github.com/" rel="nofollow noopener noreferrer"><i style="font-style:normal"  class="fab fa-fw fa-github-square" aria-hidden="true"></i> GitHub</a>&nbsp;&nbsp;&nbsp;<a href="https://twitter.com/rikenaiptlt" rel="nofollow noopener noreferrer"><i style="font-style:normal" class="fab fa-fw fa-twitter-square" aria-hidden="true"></i> Twitter</a></li>
              </ul>
            </div>
          </div>
          <div class="page__footer-copyright" style="padding-left: 30px; padding-right: 30px; color:#808080">© 2023 Tensor Learning Team. Powered by <a href="https://jekyllrb.com" rel="nofollow">Jekyll</a>.
          </div>
        </div>
      </div>
    </div>
