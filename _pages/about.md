---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
/* Float four columns side by side */
.column {
  float: left;
  width: 25%;
  padding: 0 10px;
}

/* Remove extra left and right margins, due to padding in columns */
.row {margin: 0 -5px;}

/* Clear floats after the columns */
.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Style the counter cards */
.card {
<!--   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2); /* this adds the "card" effect */ -->
  padding: 16px;
<!--   text-align: center; -->
<!--   background-color: #f1f1f1; -->
}

/* Responsive columns - one column layout (vertical) on small screens */
@media screen and (max-width: 600px) {
  .column {
    width: 100%;
    display: block;
    margin-bottom: 20px;
  }
}
  
a:link {
  text-decoration: none;
}
</style>

I am currently a PhD student in the <a href="https://cs.unc.edu">Computer Science Department</a> at the <a href="https://www.unc.edu">University of North Carolina at Chapel Hill</a>, working with Prof. <a href="https://cs.unc.edu/person/daniel-szafir">Daniel Szafir</a>. I also completed my MS in <a href="https://cs.unc.edu">Computer Science</a> from the <a href="https://www.unc.edu">University of North Carolina at Chapel Hill</a> in May 2023. My research centers on Human-Robot Interaction and Long Horizon Reasoning in Robotics, specifically building functionalities to improve Robot Long Horizon Reasoning and designing systems which allow users to interact with such robots. In my recent work, we designed and evaluated a interactive and multimodal end-user robot programming system to allow users to author and visualize reactive robot behavior. I have developed an <a href="https://maitreygram.github.io/publications/Scene-aware-language-planner">approach</a> utilizing Large Language Models to convert high-level tasks into environmentally-aware action plans for intelligent agents. Additionally, I have contributed to the design and evaluation of an immersive Cyber-Physical Control Room interface for the Boston Dynamics Spot quadruped robot. In the past I have worked with Prof. <a href="https://www.gedasbertasius.com">Gedas Bertasius</a> on studying the zero-shot performance of Vision Transformers for video object segmentation and pose propagation.

My professional journey includes research internships at <a href="https://usa.honda-ri.com">Honda Research Institute USA</a>, where I worked with the Intelligent Robotics Research team to build intelligent systems to assist robot teleoperators. Prior to that I worked at <a href="https://www.mastercard.co.in/en-in.html">AI Garage, Mastercard</a>, India, where I focused on Graph Machine Learning to generate contextual embeddings for credit cards and merchants. I also interned at <a href="https://research.samsung.com/sri-b">Samsung Research Institute, Bangalore</a> where I worked in the Computer Vision team of the Advanced Technology Lab.

Prior to my graduate studies, I completed my Bachelors in Technology in <a href="https://www.cse.iitb.ac.in">Computer Science</a> from the <a href="https://www.iitb.ac.in">Indian Institute of Technology, Bombay</a>, where I collaborated with Prof. <a href="https://www.cse.iitb.ac.in/~ajitvr">Ajit Rajwade</a> on 3D Reconstruction in Cryogenic Electron Microscopy for my <a href="https://maitreygram.github.io/thesis/BTP_Report_2.pdf">Undergraduate thesis</a>. I also served as the Software team lead for The <a href="https://iitbmartian.github.io">The IIT Bombay Mars Rover Team</a>, where I worked on building rovers capable of traversing on Mars like terrain.

# Recent Publications

<div class="row">
  <div class="column">
    <div class="card">
      <img alt="interface" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/b0b0d6d2-2925-4dce-a160-88c47896a238"/>
    </div>
  </div>
  <div class="column" style="width: 75%;">
    <div class="card">
      <a href="https://maitreygram.github.io/publications/llm_hrc">Human Robot Collaboration with Few-Shot LLM Robot Models</a>
    </div>
    <div class="card">
      <b>Maitrey Gramopadhye</b>, Daniel Szafir
    </div>
    <div class="card">
      <i>HIRL | HRI, 2024</i>
  </div>
</div>
<br>

<div class="row">
  <div class="column">
    <div class="card">
      <img alt="interface" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/834f53a9-66e5-4303-b088-5bd8b7320ee5"/>
    </div>
  </div>
  <div class="column" style="width: 75%;">
    <div class="card">
      <a href="https://maitreygram.github.io/publications/mr_interface_mixed_team">The Cyber-Physical Control Room: A Mixed Reality Interface for Mobile Robot Teleoperation and Human-Robot Teaming</a>
    </div>
    <div class="card">
      Michael E. Walker, <b>Maitrey Gramopadhye</b>, Bryce Ikeda, Jack Burns, Daniel Szafir
    </div>
    <div class="card">
      <i>HRI, 2024</i>
  </div>
</div>
<br>



<div class="row">
  <div class="column">
    <div class="card">
      <img alt="system diagram" src="https://user-images.githubusercontent.com/24911348/195924327-b4230fe0-e6ec-4cfe-acf5-3ebf3db022a9.png"/>
    </div>
  </div>
  <div class="column" style="width: 75%;">
    <div class="card">
      <a href="https://maitreygram.github.io/publications/Scene-aware-language-planner">Generating Executable Action Plans with Environmentally-Aware Language Models</a>
    </div>
    <div class="card">
      <b>Maitrey Gramopadhye</b>, Daniel Szafir
    </div>
    <div class="card">
      <i>IROS, 2023</i>
    </div>
    <div class="card">
      <i><a href="https://arxiv.org/abs/2210.04964">paper</a>, <a href="https://github.com/hri-ironlab/scene_aware_language_planner">code</a></i>
    </div>
  </div>
</div>
<br>



<div class="row">
  <div class="column">
    <div class="card">
      <img alt="interface design" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/6ff2cc18-96cf-4b6e-a689-eba30d6efac8"/>
    </div>
  </div>
  <div class="column" style="width: 75%;">
    <div class="card">
      <a href="https://maitreygram.github.io/publications/VR-or-not">Assessing the Impact of VR Interfaces in Human-Drone Interaction</a>
    </div>
    <div class="card">
      <b>Maitrey Gramopadhye</b>, Arran Zeyu Wang, Leonard Shearer, Tony Qin and Daniel Szafir
    </div>
    <div class="card">
      <i>XR-ROB | IROS, 2023</i>
    </div>
    <div class="card">
      <i><a href="https://maitreygram.github.io/papers/VR_or_not_XR_ROB_23.pdf">paper</a></i>
    </div>
  </div>
</div>
<br>



<div class="row">
  <div class="column">
    <div class="card">
      <img src="https://user-images.githubusercontent.com/24911348/195767144-15cb4b40-5808-4739-9d87-657bdf465190.png" alt="CuRL system diagram"/>
    </div>
  </div>
  <div class="column" style="width: 75%;">
    <div class="card">
      <a href="https://maitreygram.github.io/publications/CuRL">CuRL: Coupled Representation Learning of Cards and Merchants to Detect Transaction Frauds</a>
    </div>
    <div class="card">
      <b>Maitrey Gramopadhye</b>, Shreyansh Singh, Kushagra Agarwal, Nitish Srivasatava, Alok Singh, Siddhartha Asthana and Ankur Arora
    </div>
    <div class="card">
      <i>ICANN, 2021</i>
    </div>
    <div class="card">
      <i><a href="https://link.springer.com/chapter/10.1007/978-3-030-86383-8_2">paper</a></i>
    </div>
  </div>
</div>

<!-- <img width="200" alt="system diagram" src="https://user-images.githubusercontent.com/24911348/195924327-b4230fe0-e6ec-4cfe-acf5-3ebf3db022a9.png" align="left"/>
<a href="https://arxiv.org/abs/2210.04964" style="text-decoration:none">Generating Executable Action Plans with Environmentally-Aware Language Models</a> \
**Maitrey Gramopadhye**, Daniel Szafir \
*arXiv, 2022* \

<img src="https://user-images.githubusercontent.com/24911348/195767144-15cb4b40-5808-4739-9d87-657bdf465190.png" alt="CuRL system diagram" width="200" align="left"/>
<a href="https://link.springer.com/chapter/10.1007/978-3-030-86383-8_2" style="text-decoration:none">CuRL: Coupled Representation Learning of Cards and Merchants to Detect Transaction Frauds</a> \
**Maitrey Gramopadhye**, Shreyansh Singh, Kushagra Agarwal, Nitish Srivasatava, Alok Singh, Siddhartha Asthana and Ankur Arora \
*ICANN, 2021* -->
