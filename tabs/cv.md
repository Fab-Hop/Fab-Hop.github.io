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
      end_date: "31.03.2023"
      company: "FIZ - Karlsruhe"
      description: "Research on Zero-Shot Text Classification using Knowledge Graphs as auxiliary information as well as development of ontologies and Knowledge Graphs for research data management."
    - title: "Thesis Student (Master of Science)"
      start_date: "01.03.2018"
      end_date: "30.09.2018"
      company: "Bosch Global Software Technologies Pvt. Ltd."
      description: "Exploration of features for recognition of near-duplicate reports based on distributional semantics and transfer learning."
    - title: "Research Assistant"
      start_date: "01.08.2017"
      end_date: "28.02.2018"
      company: "Fraunhofer Institute of Optronics, System Technologies and Image Exploitation IOSB"
      description: "Appending virtual reality scenes with foreground objects of an IP camera."
    - title: "Thesis Student (Bachelor of Science)"
      start_date: "01.08.2016"
      end_date: "28.02.2017"
      company: "Robert Bosch GmbH"
      description: "Research on video based smoke detection for optical thin smoke."
  teaching_title: "Teaching"
  teaching_color: "#cce6ff"
  teaching_list: 
    - title: "Information Service Engineering"
      type: "lecture"
      start_date: "01.04.2020"
      end_date: "31.08.2022"
      institute: "Karlsruhe Institute of Technology"
      role: "Teaching Assistant"
      description: ""
    - title: "Knowledge Graphs"
      type: "mooc"
      start_date: ""
      end_date: ""
      institute: ""
      role: "Teaching Assistant"
      description: ""
    - title: "Bachelor Thesis: "
      type: "thesis"
      start_date: ""
      end_date: ""
      institute: ""
      role: "Thesis Supervisor"
      description: ""
      

  education_title: "Education"
  education_color: "#cce6ff"
  education_list:
    - title: "Master of Science (Computer Science)"
      start_date: "01.03.2017"
      end_date: "31.10.2018"
      university: "University of Applied Sciences Karlsruhe"
      description: "Overall mark: very good (1.2) with distinction, Courses taken (among others): Pattern Recognition, Unsupervised Learning, Photogrammetry"
    - title: "Bachelor of Science (Computer Science)"
      start_date: "01.09.2013"
      end_date: "28.02.2018"
      university: "University of Applied Sciences Karlsruhe"
      description: "Overall mark: very good (1.2) with distinction, Courses taken (among others): Computer Vision, Embedded Systems, Robotics"

  skills_title: "Skills"



---
