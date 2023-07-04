---
layout: about
title: about
permalink: /
subtitle:

profile:
  align: right
  image: profile_pic.png
  image_circular: false # crops the image to make it circular
  address:
news: False # includes a list of news items
latest_posts: False # includes a list of the newest posts
selected_papers: False # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
---

I am a Graduate Researcher/Software Engineer at the [METU Center for Image Analysis](https://ogam.metu.edu.tr). Additionally, I am working as a Research Assistant and pursuing my Master's studies at [METU](https://eee.metu.edu.tr), under the supervision of [Aydın Alatan](https://eee.metu.edu.tr/personel/aydin-alatan). My research is primarily focused on solving the multiple object tracking problem. To tackle this challenge effectively, I am developing a method that utilizes graph neural networks. I am particularly interested in the research of graph machine learning. Additionally, I have a background in signal processing, which was my major during my Bachelor's studies.

<style>
  .list-container {
    display: flex;
    gap: 120px;
  }
  
  .list-title {
    font-weight: bold;
    font-size: 22px;
  }
  
  ul {
    /* list-style: none; */
    padding-left: 0;
  }

  .list-2 span.subtext {
    font-size: 14px; /* Adjust the font size of the subtext */
    font-weight: normal;
    color: #777888;
    display: block;
    /* margin-top: 5px; Adjust the spacing between item and subtext */
    margin-left: 20px; /* Adjust the spacing between item and subtext */
  }
  
</style>

<div class="list-container">

  <div>
    <h2 class="list-title">Interests</h2>
    <ul style="padding-left:20px">
      <li>Visual Tracking</li>
      <li>Trajectory Prediction</li>
      <li>Link Prediction</li>
      <li>Graph Representation Learning</li>
    </ul>
  </div>

  <div>
    <h2 class="list-title">Education</h2>
    <ul class="list-2">
    <li style="font-size:12px" class="fa">&#xf19d;   
     </li> <b>MSc in Electrical-Electronics Eng.,2023 </b> 
     <span class="subtext">Middle East Technical University</span>
    <li style="font-size:12px" class="fa">&#xf19d;   
     </li> <b>BSc in Electrical-Electronics Eng.,2021 </b> 
     <span class="subtext">Middle East Technical University</span>
    </ul>
  </div>

</div>

<br>

### **Projects**

{% if site.data.repositories.github_repos %}

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
