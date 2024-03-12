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

<p>Michael E. Walker, Maitrey Gramopadhye, Bryce Ikeda, Jack Burns, Daniel Szafir</p>
<br>
<div class="card">
  <video width="100%" controls>
    <source src="/images/interface_demo_540.mp4" type="video/mp4">
  Your browser does not support the video tag.
  </video>
</div>
<br>

In this work, we present the design and evaluation of an immersive Cyber-Physical Control Room interface for remote mobile robots that provides users with both robot-egocentric and robot-exocentric 3D perspectives. We evaluate the Cyber-Physical Control room against a traditional robot interface in a mock disaster response scenario that features a mixed human-robot field team. In our evaluation, we found that the Cyber-Physical Control Room improved robot operator effectiveness by 28% while navigating a complex warehouse environment and performing a visual search. The Cyber-Physical Control Room also enhanced various aspects of human-robot teaming, including social engagement, the ability of a remote robot teleoperator to track their human partner in the field, and opinions of human teammate leadership qualities.

<div class="row">
  <div class="column" style="width: 50%;">
    <div class="card">
      <video controls style="width: 95%;">
        <source src="/images/spot_720.mp4" type="video/mp4">
      Your browser does not support the video tag.
      </video>
    </div>
    <div class="card">
      <p>The robot platform used - Boston Dynamics Spot, with custom sensor stack</p>
    </div>
  </div>
  <div class="column" style="width: 50%;">
    <div class="card">
      <video controls style="width: 95%;">
        <source src="/images/warehouse_540.mp4" type="video/mp4">
      Your browser does not support the video tag.
      </video>
    </div>
    <div class="card">
      <p>Tour of the warehouse used for the mock disaster response study</p>
    </div>
  </div>
</div>
<br>

## Interface Design
<div class="card">
  <img alt="interface" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/834f53a9-66e5-4303-b088-5bd8b7320ee5"/>
</div>
<br>
<div class="card">
  <p>The design of the augmented virtuality interface began with the creation of a virtual environment that provided enough space for users to comfortably walk around the entirety of a 3D reconstruction of a large indoor room. Additionally, the size of the environment matched the size of the real-life operator environment used in the experiment evaluation. The skybox was shaded black to provide the greatest contrast between the rendered sensor data and the virtual environment background. Stereo video and point cloud data were processed, transmitted, and rendered in real time; therefore, the system did not require prior information about a robot’s remote and potentially unknown environment.</p>
</div>
<div class="card">
  <p>To provide users with a robot-egocentric perspective within the interface, an External Sensor Images and Video VDE was added to the virtual environment. To make the images 3D to the robot operator, both the left and right video streams, transmitted from a stereo camera mounted on the robot, were rendered within the interface simultaneously. A small horizontal offset was added between the video streams, while the left video stream was masked (i.e., made invisible) to the user’s right eye, and the right video stream was masked to the left eye. In this way, each eye only sees one of the offset images, which allowed users to see the video stream as 3D via stereopsis. Additionally, we wanted to ensure robot operators were able to freely view the 3D reconstruction of the environment from any angle without losing sight of the video stream. Therefore, the panels holding the video stream were programmed to slide on the rails that encircled the virtual environment to automatically center in front of the user.</p>
</div>
<div class="card">
  <p>An Environment Digital Twin VDE was added to the interface to provide a robot-exocentric perspective within the interface. This digital twin took the form of a dense point cloud, rendered in the center of the virtual environment, that was generated from streamed laser scan data collected by the robot. Users were able to scale the reconstruction up (to allow for more detailed searching) or down (creating a minimap environment summary or top-down bird’s eye view) in size. Within the point cloud a Visualization Robot VDE that acted in the role of an External Robot Pose VDE and Robot Location VDE. The Visualization Robot was accurately positioned within the point cloud with an accurate pose that up- dated in real time to allow users to better understand where the robot is facing and its current operational status.</p>
</div>
<br>

## Experimental Task
<div class="card">
  <p>We designed a mock disaster scenario in which a hurricane had damaged a chemical storage facility. To limit human exposure to the hazardous site, a mixed human-robot team was assembled to act as first responders. This team consisted of three members: (1) a human fieldworker, acted out by an experimental confederate, working on-site at the facility; (2) a mobile ground robot working on-site at the facility; and (3) a remote participant that remotely teleoperated the robot.Both team members independently moved through the warehouse to complete their own tasks. The teams’ objectives were to: (1) investigate the buildings’ safety (structural stability, risk of electrical fires, etc.); (2) ensure there are no chemical leaks; and (3) locate objects of interest within the building for extraction.</p>
</div>
<div class="card">
  <p>The participant was tasked with teleoperating the robot to find objects of interest throughout the building. In a cohesive disaster response narrative, mission command would inform the participant about which objects to locate sequentially. The objects were: (1) a chemical container; (2) electrical switchboard; (3) fire extinguisher; (4) furnace; (5) box of fuses; and (6) computer hard drive. While the robot operator (i.e., experimental participant) searched for objects, the human fieldworker (i.e., experimental confederate) scanned the building’s foundations and electrical signals with a handheld device to analyze the current ‘on-the-ground’ situation, report back to mission command, and receive further instructions based on the information sent. Each time the participant located an object, they had to then search for and locate their fieldworker partner, who was also independently moving throughout the working area, to discuss the next course of action (i.e., what object to find next within the mock disaster narrative). This search and report process repeated six times until all objects were been found which marked the area as secured for the secondary cleanup team.
</p>
</div>
<br>

## Results

<div class="row">
  <div class="column" style="width: 33%;">
    <div class="card">
      <img alt="Total time to complete all tasks" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/34e10e27-a0a9-4684-9629-95fa2fa12c4c">
    </div>
    <br>
    <div class="card">
      <p>The Cyber-Physical Control Room improved completion time 28% over the Baseline interface</p>
    </div>
  </div>
  <div class="column" style="width: 33%;">
    <div class="card">
      <img alt="Social Engagement" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/131b4780-e7a0-4f64-bd3a-a8d9e55a6930">
    </div>
    <br>
    <div class="card">
      <p>We found that the participants that used our interface made eye-contact substantially more frequently compared to the baseline interface</p>
    </div>
  </div>
  <div class="column" style="width: 33%;">
    <div class="card">
      <img alt="Perceptions of Human Teammate Leadership Qualities" src="https://github.com/maitreygram/maitreygram.github.io/assets/24911348/ebf957ac-75cc-4e12-a29b-517ee66e5e47">
    </div>
    <br>
    <div class="card">
      <p>The Cyber-Physical Control Room enhanced the perception of the human teammate's leadership quality over the baseline interface</p>
    </div>
  </div>
</div>
