---
title: "STEP: State-Aware Task Estimation and Planning with Multi-Modal LLMs for Human-Robot Collaboration"
collection: publications
permalink: /publications/step
authors: <b>Maitrey Gramopadhye</b>, Prakash Baskaran, Xiao Liu, Songpo Li, Soshi Iba
excerpt: 'STEP is a method to enhance long-term action anticipation with multi-model large language models by explicitly estimating the state of the system and predicting the state transitions, leading to more accurate and executable robot action plans in collaborative industrial tasks.'
date: 2026-07-01
venue: 'IEEE International Conference on Robot and Human Interactive Communication (RO-MAN)'
paperurl: ''
---

<style>
/* Style the counter cards */
.column {
  float: left;
  width: 25%;
  padding: 0 10px;
}

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

<b>Maitrey Gramopadhye</b>, Prakash Baskaran, Xiao Liu, Songpo Li, Soshi Iba
<br>
<div class="card">
  <video width="100%" controls>
    <source src="/images/vid_step.mp4" type="video/mp4">
  Your browser does not support the video tag.
  </video>
</div>
<br>

[View the paper here](https://maitreygram.github.io/papers/0345_FI.pdf)

Effective human-robot collaboration in industrial settings requires robots to understand human intentions and assist with task planning, reducing workload. Recent works have explored the use of Multi-modal Large Language Models (MM-LLMs) for task planning in such data-scarce scenarios, leveraging in-context learning to interpret user actions and generate long-horizon action plans in natural language. However, MM-LLMs inherently lack an understanding of system states and do not track state transitions, often leading to hallucinated actions that deviate from the intended goal. Additionally, generating action plans in natural language tends to limit the generated plans to a high level, introducing ambiguity in action execution. To address these limitations, we propose the State-aware Task Estimator and Planner (<b>STEP</b>), which prompts a MM-LLM to explicitly estimate the state of the system and predict the state transitions resulting from executed actions. By forecasting future states alongside actions, STEP ensures task-convergent planning while also providing additional assistance parameters necessary for executing the predicted actions. We evaluate STEP in a simulated environment using a robot assembly task. Our approach outperforms the state-of-the-art by 32.8% in action executability and 14.8% in final-state error.
