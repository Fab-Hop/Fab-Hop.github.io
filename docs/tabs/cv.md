---
layout: cv
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_cv

# publish date (used for seo)
# if not specified, site.time will be used.
#date: 2022-03-03 12:32:00 +0000

# for override items in _data/lang/[language].yml
#title: My title
#button_name: "My button"
# for override side_and_top_nav_buttons in _data/conf/main.yml
#icon: "fa fa-bath"

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-03-03 12:32:00 +0000
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# please use the "image_viewer_on" below to enable image viewer for individual pages or posts (_posts/ or [language]/_posts folders).
# image viewer can be enabled or disabled for all posts using the "image_viewer_posts: true" setting in _data/conf/main.yml.
image_viewer_on: true
# please use the "image_lazy_loader_on" below to enable image lazy loader for individual pages or posts (_posts/ or [language]/_posts folders).
# image lazy loader can be enabled or disabled for all posts using the "image_lazy_loader_posts: true" setting in _data/conf/main.yml.
image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
img: ":cv-heading.jpg"
page_data:
  main:
    header: "Curriculum Vitae"
    info: "Test"

  category: 
    - title: "Work Experience"
      type: id_work
      color: "#cce6ff"
    - title: "Teaching"
      type: id_teaching
      color: "#cce6ff"
    - title: "Education"
      type: id_education
      color: "#cce6ff"
      
  work_title: "Work Experience"
  work_color: "#cce6ff"
  work_list:
    - title: "Junior Researcher"
      start_date: "01.06.2019"
      end_date: "01.03.2023"
      company: "FIZ - Karlsruhe"
      description: "Research on Zero-Shot Text Classification using Knowledge Graphs as auxiliary information as well as development of ontologies and Knowledge Graphs for research data management."
    - title: "Thesis Student (Master of Science)"
      start_date: ""
      end_date: ""
      company: ""
      description: ""
    - title: "Research Assistant"
      start_date: ""
      end_date: ""
      company: ""
      description: ""
    - title: "Thesis Student (Bachelor of Science)"
      start_date: ""
      end_date: ""
      company: ""
      description: ""
  teaching_title: "Teaching"
  teaching_color: "#cce6ff"
  teaching_list: 
    - title: ""

  education_title: "Education"
  education_color: "#cce6ff"
  education_list:
    - title: "Master of Science (Computer Science)"
      start_date: ""
      end_date: ""
      university: "University of Applied Sciences Karlsruhe"
      description: ""
    - title: "Bachelor of Science (Computer Science)"
      start_date: ""
      end_date: ""
      university: "University of Applied Sciences Karlsruhe"
      description: ""



---
