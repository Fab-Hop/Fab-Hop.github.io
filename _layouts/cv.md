---

layout: default
# CV page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}

{%- assign cv_data = page.page_data | default: site.data.content.links[lng].page_data -%}

{%- if page.img %}
  {%- if site.data.conf.others.cv.header_img_with_img_tag == true -%}
    {%- capture home_img_tag -%} <img src="{{ page.img }}" /> {%- endcapture -%}
    {%- capture home_img_background_style -%} style="height: unset;" {%- endcapture -%}
  {% else %}
    {%- capture home_img_background_style -%} style="background-image:url('{{ page.img }}');" {%- endcapture -%}
  {%- endif -%}
{%- endif -%}


<div class="multipurpose-container cv-heading-container">
  <div class="home-heading" {{ home_img_background_style}}>
  {{ home_img_tag }}
  </div>
  <h1>{{ cv_data.main.header | default: "CV" }}</h1>
  <p>{{ cv_data.main.info | default: "No data, check page_data in [language]/tabs/cv.md front matter or _data/content/cv/[language].yml" }}</p>
  <div class="multipurpose-button-wrapper">
    <a href="#work" role="button" class="multipurpose-button link-buttons" style="background-color:{{ cv_data.work_color }};">{{ cv_data.work_title }}</a>
    <a href="#teaching" role="button" class="multipurpose-button link-buttons" style="background-color:{{ cv_data.teaching_color }};">{{ cv_data.teaching_title }}</a>
    <a href="#education" role="button" class="multipurpose-button link-buttons" style="background-color:{{ cv_data.education_color }};">{{ cv_data.education_title }}</a>
  </div>
</div>

<div class="multipurpose-container cv-container" id="work" style="border-left-color:{{ cv_data.work_color }};">
  <h2>{{ cv_data.work_title}}</h2>
  <table class="table {{ hover_class }}">
    <thead>
      <tr>
        <th>{{ site.data.lang[lng].cv.start_text}}</th>
        <th>{{ site.data.lang[lng].cv.end_text}}</th>
        <th>{{ site.data.lang[lng].cv.job_text }}</th>
        <th>{{ site.data.lang[lng].cv.company_text }}</th>
      </tr>
    </thead>
    <tbody>
      {%- for list in cv_data.work_list %}
        <tr >
          <td rowspan="2" style='vertical-align:middle'>
            <p>{{list.start_date}}</p>
          </td>
          <td rowspan="2" style='vertical-align:middle'>
            <p>{{list.end_date}}</p>
          </td>
          <td>
            <p><b>{{list.title}}</b></p>
          </td>
          <td>
            <p>{{ list.company }}</p>
          </td>
        </tr>
        <tr>
          <td colspan="2">
            <p>{{ list.description }}</p>
          </td>
        </tr>
      {%- endfor %}
    </tbody>
  </table>
</div>

<div class="multipurpose-container cv-container" id="teaching" style="border-left-color:{{ cv_data.teaching_color }};">
  <h2>{{ cv_data.teaching_title}}</h2>
  <table class="table {{ hover_class }}">
    <thead>
      <tr>
        <th>{{ site.data.lang[lng].cv.start_text}}</th>
        <th>{{ site.data.lang[lng].cv.end_text}}</th>
        <th>{{ site.data.lang[lng].cv.job_text }}</th>
        <th>{{ site.data.lang[lng].cv.university_text }}</th>
      </tr>
    </thead>
    <tbody>
      {%- for list in cv_data.teaching_list %}
        <tr >
          <td rowspan="2">
            <p>{{list.start_date}}</p>
          </td>
          <td rowspan="2">
            <p>{{list.end_date}}</p>
          </td>
          <td>
            <p><b>{{list.title}}</b></p>
          </td>
          <td>
            <p>{{ list.institute }}</p>
          </td>
        </tr>
        <tr>
          <td colspan="2">
            <p>{{ list.description }}</p>
          </td>
        </tr>
      {%- endfor %}
    </tbody>
  </table>
</div>

<div class="multipurpose-container cv-container" id="education" style="border-left-color:{{ cv_data.education_color }};">
  <h2>{{ cv_data.education_title}}</h2>
  <table class="table {{ hover_class }}">
    <thead>
      <tr>
        <th>{{ site.data.lang[lng].cv.start_text}}</th>
        <th>{{ site.data.lang[lng].cv.end_text}}</th>
        <th>{{ site.data.lang[lng].cv.degree_text }}</th>
        <th>{{ site.data.lang[lng].cv.university_text }}</th>
      </tr>
    </thead>
    <tbody>
      {%- for list in cv_data.education_list %}
        <tr >
          <td rowspan="2">
            <p>{{list.start_date}}</p>
          </td>
          <td rowspan="2">
            <p>{{list.end_date}}</p>
          </td>
          <td>
            <p><b>{{list.title}}</b></p>
          </td>
          <td>
            <p>{{ list.university }}</p>
          </td>
        </tr>
        <tr>
          <td colspan="2">
            <p>{{ list.description }}</p>
          </td>
        </tr>
      {%- endfor %}
    </tbody>
  </table>
</div>
<div class="multipurpose-container cv-container" id="skill" style="border-left-color:{{ cv_data.education_color }};">
  <h2>{{ cv_data.skills_title}}</h2>
</div>
