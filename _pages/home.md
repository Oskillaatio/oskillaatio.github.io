---
title: "Oskillaatio – Helsingin yliopiston fysikaalisten tieteiden alumnit ry"
layout: splash
permalink: /
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#ff00ff"
  overlay_filter: "0"
  overlay_image: /assets/images/sinit_harmaatausta.png
  actions:
    - label: "Liity jäseneksi"
      url: "https://forms.gle/EEA1BEzemyVxmqceA"
excerpt: "Oskillaatio on kaikkien Helsingin yliopiston fysikaalisten tieteiden alumnien yhdistys"
feature_row:
  - image_path: /assets/images/oskillaatio-logo.png
    alt: "placeholder image 1"
    title: "Liity jäseneksi"
    url: https://forms.gle/EEA1BEzemyVxmqceA
    excerpt: "Uudet jäsenhakemukset käsitellään seuraavassa hallituksen kokouksessa." #"Liity yhdistyksen jäseneksi täyttämällä jäsenlomake"
    btn_label: "Jäsenhakulomake"
    btn_class: "btn--info"
  - image_path: /assets/images/oskillaatio-logo.png
    # image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    # alt: "placeholder image 2"
    title: "Tulevat tapahtumat"
    excerpt: "Lisää Oskillaation sähköinen kalenteri itsellesi."
    url: "/tapahtumat/"
    btn_label: "Tapahtumakalenteri"
    btn_class: "btn--info"
  - image_path: /assets/images/oskillaatio-logo.png
    title: "Tiedotuskanavat"
    url: /yhteystiedot/
    btn_label: "Seuraa yhdistystä"
    btn_class: "btn--info"    
    excerpt: "Oskillaation toiminnasta tiedotetaan sähköpostilistalla, [Facebook-ryhmässä](https://www.facebook.com/groups/5306881863/) ja [Telegram-keskustelussa](https://t.me/+fb_BwM_D0SUxYjU0)."
# feature_row2:
#   - image_path: /assets/images/oskillaatio-logo.jpg
#     alt: "placeholder image 2"
#     title: "Placeholder Image Left Aligned"
#     excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
#     url: "#test-link"
#     btn_label: "Read More"
#     btn_class: "btn--primary"
# feature_row3:
#   - image_path: /assets/images/oskillaatio-logo.jpg
#     alt: "placeholder image 2"
#     title: "Placeholder Image Right Aligned"
#     excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
#     url: "#test-link"
#     btn_label: "Read More"
#     btn_class: "btn--primary"
# feature_row4:
#   - image_path: /assets/images/oskillaatio-logo.jpg
#     alt: "placeholder image 2"
#     title: "Placeholder Image Center Aligned"
#     excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
#     url: "#test-link"
#     btn_label: "Read More"
#     btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

<div class="feature__wrapper">
   {% for post in site.posts limit:3 %}
   <div class="feature__item">
      <div class="archive__item">
         <div class="archive__item-body">
            <h3 class="archive__item-title"><a href="{{ site.baseurl }}{{ post.url}}" rel="permalink">{{ post.title }}</a></h3>
            <div class="archive__item-excerpt">
               <p>{{ post.excerpt | markdownify }}</p>
               <div style="position:aboslute;bottom:0;right:0" align="right"><b>{{post.date | date: "%d.%m.%Y"}}</b></div>
            </div>
         </div>
      </div>
   </div>
   {% endfor %}
</div>

{% include feature_row %}

<!-- {% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %} -->
