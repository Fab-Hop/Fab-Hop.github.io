---
# Mr. Green Jekyll Theme (https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme)
# Copyright (c) 2022 Mr. Green's Workshop https://www.MrGreensWorkshop.com
# Licensed under MIT

layout: default
# About page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}

{%- assign imprint_data = page.page_data | default: site.data.content.links[lng].page_data -%}

{%- if page.img %}
  {%- if site.data.conf.others.publications.header_img_with_img_tag == true -%}
    {%- capture home_img_tag -%} <img src="{{ page.img }}" /> {%- endcapture -%}
    {%- capture home_img_background_style -%} style="height: unset;" {%- endcapture -%}
  {% else %}
    {%- capture home_img_background_style -%} style="background-image:url('{{ page.img }}');" {%- endcapture -%}
  {%- endif -%}
{%- endif -%}


<div class="multipurpose-container imprint-container">
  <h1>{{imprint_data.main.header}}</h1>
  <hr>
  <div class="row about-main">
    {{ content }}
  </div>
</div>
