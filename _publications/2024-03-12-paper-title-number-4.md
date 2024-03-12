---
title: "The Cyber-Physical Control Room: A Mixed Reality Interface for Mobile Robot Teleoperation and Human-Robot Teaming"
collection: publications
permalink: /publications/mr_interface_mixed_team
authors: Michael E. Walker, <b>Maitrey Gramopadhye</b>, Bryce Ikeda, Jack Burns, Daniel Szafir
excerpt: 'In this paper, we present the design and evaluation of an immersive Cyber-Physical Control Room interface for teleoperating remote mobile robots.'
date: 2024-03-12
venue: 'ACM/IEEE International Conference on Human Robot Interaction (HRI)'
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
    <source src="/images/interface_demo_540.mp4" type="video/mp4">
  Your browser does not support the video tag.
  </video>
</div>
<br>

In this work, we present the design and evaluation of an immersive Cyber-Physical Control Room interface for remote mobile robots that provides users with both robot-egocentric and robot-exocentric 3D perspectives. We evaluate the Cyber-Physical Control room against a traditional robot interface in a mock disaster response scenario that features a mixed human-robot field team. In our evaluation, we found that the Cyber-Physical Control Room improved robot operator effectiveness by 28% while navigating a complex warehouse environment and performing a visual search. The Cyber-Physical Control Room also enhanced various aspects of human-robot teaming, including social engagement, the ability of a remote robot teleoperator to track their human partner in the field, and opinions of human teammate leadership qualities.

<div class="row">
  <div class="column" width="49%">
    <div class="card">
      <video width="49%" controls>
        <source src="/images/spot_720.mp4" type="video/mp4">
      Your browser does not support the video tag.
      </video>
    </div>
<!--     <div class="card">
      <p>The robot platform used - Boston Dynamics Spot, with custom sensor stack</p>
    </div> -->
  </div>
  <div class="column" width="49%">
    <div class="card">
      <video width="49%" controls>
        <source src="/images/warehouse_540.mp4" type="video/mp4">
      Your browser does not support the video tag.
      </video>
    </div>
<!--     <div class="card">
      <p>Tour of the warehouse used for the mock disaster response study</p>
    </div> -->
  </div>
</div>
<br>

<h3>Interface Design</h3>

<div class="row">
  <div class="column">
    <div class="card">
      <img alt="interface" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/834f53a9-66e5-4303-b088-5bd8b7320ee5"/>
    </div>
    <br>
    <div class="card">
      <p>The design of the augmented virtuality interface began with the creation of a virtual environment that provided enough space for users to comfortably walk around the entirety of a 3D reconstruction of a large indoor room. Additionally, the size of the environment matched the size of the real-life operator environment used in the experiment evaluation. The skybox was shaded black to provide the greatest contrast between the rendered sensor data and the virtual environment background. Stereo video and point cloud data were processed, transmitted, and rendered in real time; therefore, the system did not require prior information about a robot’s remote and potentially unknown environment.</p>
    </div>
  </div>
  <div class="column">
    <div class="card">
      <p>To provide users with a robot-egocentric perspective within the interface, an External Sensor Images and Video VDE was added to the virtual environment. To make the images 3D to the robot operator, both the left and right video streams, transmitted from a stereo camera mounted on the robot, were rendered within the interface simultaneously. A small horizontal offset was added between the video streams, while the left video stream was masked (i.e., made invisible) to the user’s right eye, and the right video stream was masked to the left eye. In this way, each eye only sees one of the offset images, which allowed users to see the video stream as 3D via stereopsis. Additionally, we wanted to ensure robot operators were able to freely view the 3D reconstruction of the environment from any angle without losing sight of the video stream. Therefore, the panels holding the video stream were programmed to slide on the rails that encircled the virtual environment to automatically center in front of the user.</p>
    </div>
    <br>
    <div class="card">
      <p>An Environment Digital Twin VDE was added to the interface to provide a robot-exocentric perspective within the interface. This digital twin took the form of a dense point cloud, rendered in the center of the virtual environment, that was generated from streamed laser scan data collected by the robot. Users were able to scale the reconstruction up (to allow for more detailed searching) or down (creating a minimap environment summary or top-down bird’s eye view) in size. Within the point cloud a Visualization Robot VDE that acted in the role of an External Robot Pose VDE and Robot Location VDE. The Visualization Robot was accurately positioned within the point cloud with an accurate pose that up- dated in real time to allow users to better understand where the robot is facing and its current operational status.</p>
    </div>
  </div>
</div>
