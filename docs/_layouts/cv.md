---

layout: default
# CV page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}

{%- assign cv_data = page.page_data | default: site.data.content.links[lng].page_data -%}

<div class="multipurpose-container cv-heading-container">
  <h1>{{ cv_data.main.header | default: "CV2" }}</h1>
  <p>{{ cv_data.main.info | default: "No data, check page_data in [language]/tabs/cv.md front matter or _data/content/cv/[language].yml" }}</p>
  <div class="multipurpose-button-wrapper">
    {%- for category in cv_data.category %}
      <a href="#{{ category.type }}" role="button" class="multipurpose-button link-buttons" style="background-color:{{ category.color }};">{{ category.title }}</a>
    {% endfor -%}
  </div>
</div>

{%- if site.data.conf.others.links.use_rows_as_link -%}{%- assign hover_class = "table-hover" -%}{%- endif -%}
{%- for category in cv_data.category %}
<div class="multipurpose-container cv-container" id="{{ category.type }}" style="border-left-color:{{ category.color }};">
  <h2>{{ category.title }}</h2>
  <table class="table {{ hover_class }}">
    <thead>
      <tr>
        <th>{{ site.data.lang[lng].cv.cv_text }}</th>
        <th>{{ site.data.lang[lng].cv.info_text }}</th>
      </tr>
    </thead>
    <tbody>
      {%- for list in cv_data.list %}
        {%- if list.type != category.type %}{% continue %}{% endif -%}
        {%- if site.data.conf.others.cv.use_rows_as_link -%}
          {%- capture link_onclick -%} onclick="openURL('{{ list.url }}');" style="cursor: pointer;" {%- endcapture -%}
          {%- capture link_url -%} <b>{{ list.title }}</b> {%- endcapture -%}
        {% else %}
          {%- assign link_onclick = nil -%}
          {%- capture link_url -%} <a href="{{ list.url }}" target="_blank" rel="noopener noreferrer"><b>{{ list.title }}</b></a> {%- endcapture -%}
        {%- endif %}
        <tr class="link-item" {{ link_onclick }}>
          <td>
            <p>{{ link_url }}</p>
          </td>
          <td>
            <p>{{ list.info }}</p>
          </td>
        </tr>
      {%- endfor %}
    </tbody>
  </table>
</div>
{% endfor %}
