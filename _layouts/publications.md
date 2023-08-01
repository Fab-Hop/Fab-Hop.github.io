---
layout: default
# Publications page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}

{%- assign publication_data = page.page_data | default: site.data.content.links[lng].page_data -%}

{%- if page.img %}
  {%- if site.data.conf.others.publications.header_img_with_img_tag == true -%}
    {%- capture home_img_tag -%} <img src="{{ page.img }}" /> {%- endcapture -%}
    {%- capture home_img_background_style -%} style="height: unset;" {%- endcapture -%}
  {% else %}
    {%- capture home_img_background_style -%} style="background-image:url('{{ page.img }}');" {%- endcapture -%}
  {%- endif -%}
{%- endif -%}


<div class="multipurpose-container publication-heading-container">
  <div class="home-heading" {{home_img_background_style}}>
    {{ publication_data.img }}
  </div>
  <h1>{{ publication_data.main.header}}</h1>
  <div class="row about-main">
    <div class="meta-container">
      {% include default/scholar-links.html -%}
    </div>
    <hr/>
    <ul>
      <li>Overall publications: {% bibliography_count --file my_publications %}</li>
      <li>Publications in conference proceedings: {% bibliography_count --file my_publications --query @inproceedings %}</li>
      <li>Publications in journals: {% bibliography_count --file my_publications --query @article %}</li>
    </ul>

  </div>
</div>

<div class="multipurpose-container publications-container">
    {{ content }}
</div>
