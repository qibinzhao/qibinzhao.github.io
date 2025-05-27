---
layout: splash
$paragraph-indent: true
permalink: /publications/064-publications/
year: 2025
type: journal
title: 'Unified multimodal multidomain polymer representation for property prediction'
authors: Q. Huang, Y. Li, L. Zhu, Q. Zhao, and W. Yu
venue: npj Computational Materials, 2025
picture: 
links:
   - type: website
     display: Website
     url: https://www.nature.com/articles/s41524-025-01652-z
  # - type: pdf
  #   display: PDF
  #   url: https://openreview.net/pdf?id=rih3hsSWx8
  # - type: code
  #   display: Code
  #   url: https://github.com/pingzaiwang/Analysis4TNN
bibtex: '@Article{Huang2025,
  author    = {Huang, Qi and Li, Yedi and Zhu, Lei and Zhao, Qibin and Yu, Wenjie},
  journal   = {npj Computational Materials},
  title     = {Unified multimodal multidomain polymer representation for property prediction},
  year      = {2025},
  issn      = {2057-3960},
  month     = may,
  number    = {1},
  volume    = {11},
  doi       = {10.1038/s41524-025-01652-z},
  publisher = {Springer Science and Business Media LLC},
}'
---

<script>
  function download_file(name, contents, mime_type) {
    // preprocessing for bibtex
  while(contents.includes("  ")) {
    contents = contents.replace(new RegExp("  ", 'g'), " ");
  }
  contents = contents.replace(new RegExp("\n", 'g'), "");
  contents = contents.split(",");
  contents = contents[0] + ",\n" + contents.slice(1, contents.length)
  contents = contents.replace(new RegExp("},", 'g'), "}");
  contents = contents.replace(new RegExp("} ", 'g'), "}");
  contents = contents.replace(new RegExp(" }", 'g'), "}");
  contents = contents.split("}");
  var final_text = ""
  for(var i=0 ; i < contents.length - 1 ; i++) {
    if(i < contents.length - 2) {
      final_text += contents[i] + "},\n "
    }
  }
  final_text = final_text.substring(0, final_text.length-3) + "\n}";
  
    mime_type = mime_type || "text/plain";
    var blob = new Blob([final_text], {type: mime_type});
    var dlink = document.createElement('a');
  document.body.appendChild(dlink);
    dlink.download = name;
    dlink.href = window.URL.createObjectURL(blob);
    dlink.onclick = function(e) {
      // revokeObjectURL needs a delay to work properly
      var that = this;
      setTimeout(function() {
          window.URL.revokeObjectURL(that.href);
      }, 1500);
    };
    dlink.click();
    dlink.remove();
    document.body.removeChild(dlink);
  }
</script>

<link rel="stylesheet" href="/assets/css/bootstrap.css">

<style>


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

td {
    border-bottom: 1px solid #fff;
}

a {
    color: #158CBA;
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

li {
    font-size: 12px;
}

.ai {
    font-family: 'Academicons';
    font-weight: 400;
    /* display: inline-block; */
    font-style: normal;
    font-variant: normal;
    text-rendering: auto;
    line-height: 1;
}
</style>

<div style="padding-bottom: 20rem;" class="container-home page__other__hero--overlay">
  <h1 style="text-transform: capitalize" class="entry-headers"> Publication </h1>
  <br>
  <tr class="paper-font" style="height:120px;">
    <td>
      {% if page.type == 'conference' %}
      <b><span style="border: 1px solid #000;">&nbsp;&#67;&nbsp;</span></b>
      {% endif %}
      {% if page.type == 'journal' %}
      <span style="border: 1px solid #000;">&nbsp;&#74;&nbsp;</span>
      {% endif %}
      &nbsp;<b><span>{{ page.title }}</span></b><br>
      <span>{{ page.authors }}</span><br>
      <i>{{ page.venue }}</i><br>
      {% if page.bibtex.size > 0 %}
      <button class="paper-btn" onclick="download_file('ref.bib', '{{ paper.bibtex }}')"><i style="font-style:normal" class="{{ site.publication_buttons['bibtex'] }}"></i>&nbsp;BibTeX</button> &nbsp;
      {% endif %}
      {% for link in page.links %}
      <a href="{{ link.url | default: '#' }}"><button class="paper-btn"><i style="font-style:normal" class="{{ site.publication_buttons[link.type] }}"></i>&nbsp;{{ link.display }}</button></a> &nbsp;
      {% endfor %}
      {% if page.note.size > 0 %}
      <br><span style="color:gray; font-size:8px;">{{ page.note }}</span>
      {% endif %}
      {% if page.specialnote.size > 0 %}
      <br><span style="color:red; font-size:8px;">{{ page.specialnote }}</span>
      {% endif %}
    </td>
  </tr> 
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
