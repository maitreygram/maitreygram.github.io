---
title: "Generating Executable Action Plans with Environmentally-Aware Language Models"
collection: publications
permalink: /publications/Scene-aware-language-planner
authors: <b>Maitrey Gramopadhye</b>, Daniel Szafir
excerpt: 'In this paper, we propose an approach to utilise large language models and convert high level tasks to environmentally-aware action plans that can be directly mapped to executable agent actions. Our approach involves integrating environmental objects and object relations as additional inputs into LLM action plan generation to provide the system with an awareness of its surroundings.'
date: 2023-05-02
venue: 'IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)'
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
  <video width="100%" controls>
    <source src="/images/Scene_aware_LLM_planner__IROS_.mp4" type="video/mp4">
  Your browser does not support the video tag.
  </video>
</div>
<br>

Large Language Models (LLMs) trained using massive text datasets have recently shown promise in generating action plans for robotic agents from high level text queries. However, these models typically do not consider the robot's environment, resulting in generated plans that may not actually be executable, due to ambiguities in the planned actions or environmental constraints. In this paper, we propose an approach to generate environmentally-aware action plans that agents are better able to execute. Our approach involves integrating environmental objects and object relations as additional inputs into LLM action plan generation to provide the system with an awareness of its surroundings, resulting in plans where each generated action is mapped to objects present in the scene. We also design a novel scoring function that, along with generating the action steps and associating them with objects, helps the system disambiguate among object instances and take into account their states. We evaluated our approach using the VirtualHome simulator and the ActivityPrograms knowledge base and found that action plans generated from our system had a 310% improvement in executability and a 147% improvement in correctness over prior work.

[paper](https://arxiv.org/abs/2210.04964), [code](https://github.com/hri-ironlab/scene_aware_language_planner), [demo](https://colab.research.google.com/drive/1WUtzFrI7pxsLoWs1PjqMZx5ewkBjKzOU?usp=sharing)

Cite this paper as:
<pre>
  <code>
    @article{gramopadhye2022generating,
    author = {Gramopadhye, Maitrey and Szafir, Daniel},
    title = {Generating Executable Action Plans with Environmentally-Aware Language Models},
    publisher = {arXiv},
    year = {2023}
    }
  </code>
</pre>
