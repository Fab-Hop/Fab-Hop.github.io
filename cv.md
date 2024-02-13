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
    info: "I am a first stage researcher with experience working in an international, heterogeneous, interdisciplinary research group. I conducted independent research on Natural Language Understanding and managed research projects on research data management. My research areas include Knowledge Graphs and Machine Learning with a focus on Zero-Shot Learning."
      
  work_title: "Work Experience"
  work_list:
    - title: "PhD Student"
      start_date: "09/2023"
      end_date: ""
      company: "Vrije Universiteit Amsterdam"
      description: "Research on combining Large Language Models and Knowledge Graphs."
    - title: "Junior Researcher"
      start_date: "06/2019"
      end_date: "03/2023"
      company: "FIZ - Karlsruhe"
      description: "Research on Zero-Shot Text Classification using Knowledge Graphs as auxiliary information as well as development of ontologies and Knowledge Graphs for research data management."
    - title: "Thesis Student"
      start_date: "03/2018"
      end_date: "09/2018"
      company: "Bosch Global Software Technologies Pvt. Ltd."
      description: "Exploration of features for recognition of near-duplicate reports based on distributional semantics and transfer learning."
    - title: "Research Assistant"
      start_date: "08/2017"
      end_date: "02/2018"
      company: "Fraunhofer Institute of Optronics, System Technologies and Image Exploitation IOSB"
      description: "Appending virtual reality scenes with foreground objects of an IP camera."
    - title: "Thesis Student"
      start_date: "08/2016"
      end_date: "02/2017"
      company: "Robert Bosch GmbH"
      description: "Research on video based smoke detection for optical thin smoke."
  teaching_title: "Teaching"
  teaching_list: 
    - role: "Teaching Assistant"
      role_list: 
        - title: "Information Service Engineering"
          start_date: "04/2020"
          end_date: "08/2022"
          institute: "Karlsruhe Institute of Technology"
          description: "Lecture on fundamentals of natural language processing, knowledge mining, linked data engineering and information retrieval."
        - title: "MOOC: Knowledge Graphs"
          start_date: "08/2020"
          end_date: "12/2020"
          institute: "Hasso-Platner Institute"
          description: "Massive Open Online Course about basic semantic technologies including symbolic AI, knowledge representation with RDF, OWL and querying knowledge graphs via SPARQL."
    - role: "Thesis Supervisor"
      role_list:
        - title: "Bachelor Thesis"
          start_date: "05/2020"
          end_date: "12/2020"
          institute: "Karlsruhe Institute of Technology"
          description: "Evaluation of methods based on large language models for fine-grained text classification."
        - title: "Bachelor Thesis"
          start_date: "05/2020"
          end_date: "09/2020"
          institute: "Karlsruhe Institute of Technology"
          description: "Knowledge extraction from structured Wikipedia list pages using regular expressions."
     

  education_title: "Education"
  education_list:
    - title: "Master of Science"
      subject: "Computer Science"
      start_date: "03/2017"
      end_date: "10/2018"
      university: "University of Applied Sciences Karlsruhe"
      grade: "Overall mark: <b>very good (1.2)</b> with distinction"
      description: "Courses taken (among others): Pattern Recognition, Unsupervised Learning, Photogrammetry"
    - title: "Bachelor of Science"
      subject: "Computer Science"
      start_date: "09/2013"
      end_date: "02/2017"
      university: "University of Applied Sciences Karlsruhe"
      grade: "Overall mark: <b>very good (1.2)</b> with distinction"
      description: "Courses taken (among others): Computer Vision, Embedded Systems, Robotics"
---
