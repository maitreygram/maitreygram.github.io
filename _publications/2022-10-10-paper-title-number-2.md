---
title: "Generating Executable Action Plans with Environmentally-Aware Language Models"
collection: publications
permalink: /publication/Scene-aware-language-planner
excerpt: 'In this paper, we propose an approach to utilise large language models and convert high level tasks to environmentally-aware action plans that can be directly mapped to executable agent actions. Our approach involves integrating environmental objects and object relations as additional inputs into LLM action plan generation to provide the system with an awareness of its surroundings.'
date: 2022-10-10
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2210.04964'
---

<style>
/* Style the counter cards */
.card {
<!--   box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2); /* this adds the "card" effect */ -->
  padding: 16px;
<!--   text-align: center; -->
<!--   background-color: #f1f1f1; -->
}
  
a:link {
  text-decoration: none;
}
</style>

<div class="card">
  <video controls>
    <source src="/images/Scene_aware_LLM_planner.mp4" type="video/mp4">
  Your browser does not support the video tag.
  </video>
</div>

Large Language Models (LLMs) trained using massive text datasets have recently shown promise in generating action plans for robotic agents from high level text queries. However, these models typically do not consider the robot's environment, resulting in generated plans that may not actually be executable due to ambiguities in the planned actions or environmental constraints. In this paper, we propose an approach to generate environmentally-aware action plans that can be directly mapped to executable agent actions. Our approach involves integrating environmental objects and object relations as additional inputs into LLM action plan generation to provide the system with an awareness of its surroundings, resulting in plans where each generated action is mapped to objects present in the scene. We also design a novel scoring function that, along with generating the action steps and associating them with objects, helps the system disambiguate among object instances and take into account their states. We evaluate our approach using the VirtualHome simulator and the ActivityPrograms knowledge base. Our results show that the action plans generated from our system outperform prior work in terms of their correctness and executability by 5.3% and 8.9% respectively.

[arXiv](https://arxiv.org/abs/2210.04964)

Cite this paper as:
<pre>
  <code>
    @article{Gramopadhye2022SceneAP,
    author = {Gramopadhye, Maitrey and Szafir, Daniel},
    title = {Generating Executable Action Plans with Environmentally-Aware Language Models},
    publisher = {arXiv},
    year = {2022}
    }
  </code>
</pre>
