---
layout: splash
$paragraph-indent: true
permalink: /codes/028-codes/
year: 2025
title: 'Adversarial guided diffusion models for adversarial purification (Neural Networks, 2025)'
links:
  - type: github
    display: Github
    url: https://github.com/glin2022/AGDM
    icon: github
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
  <h1 style="text-transform: capitalize" class="entry-headers"> Code </h1>
  <h2>  </h2>
  <table class="publications">
  <tr class="paper-font">
    <td>
      <!-- <i style="font-style:normal" class="fa fa-paperclip" aria-hidden="true"></i>&nbsp; -->
      {% for link in page.links %}
      {% if link.icon == 'bibtex' %}
      <a href="{{ link.url | default: '#' }}"><button class="paper-btn">&nbsp;<i style="font-style:normal" class="{{ site.publication_buttons[link.icon] }}"></i>&nbsp;&nbsp;{{ link.display }}&nbsp;</button></a>&nbsp;
      {% endif %}
      {% if link.icon == 'github' %}
      <a href="{{ link.url | default: '#' }}"><button class="paper-btn"><i style="font-style:normal" class="{{ site.publication_buttons[link.icon] }}"></i>&nbsp;{{ link.display }}</button></a>&nbsp;
      {% endif %}
      {% endfor %}
      <b><span>{{ page.title }}</span></b>&nbsp;
    </td>
  </tr>
</table>
