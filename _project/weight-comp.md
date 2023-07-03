---
title: "Weight Compensation Mechanism for an Elastic Metamaterial"
img: projects/cover-pictures/weightComp.webp
collection: project
date: 2022-01-03
---
<p align="justify">
For the senior design project, our group worked on a weight compensation mechanism for the inertial amplification mechanism proposed by Prof. Çetin Yılmaz, in this <a href="https://journals.aps.org/prb/abstract/10.1103/PhysRevB.76.054309" target="_blank">paper</a>, who is also the advisor of our project. Check the <a href="#project-report">report</a> for more details about our contributions.
</p>

<p align="justify">
Metamaterials are artificial materials produced to have properties that go beyond properties of natural materials. They usually have periodic structures designed in such a way that they interact with their environment in unique ways. For example, a negative refractive index or a negative Poisson’s ratio. The type of metamaterial that we are interested in is elastic metamaterials with phononic band gaps. Here the term phononic refers to vibrational motion in general such as acoustic waves, elastic waves and so on. What these materials do is that they inhibit the transmission of vibration in a certain frequency range. To visualize this, imagine the left end of this material is vibrated at a frequency of 290Hz which is in the band gap. 
</p>

<div style="width:100%">
  <center>
    <video style="width:90%" muted autoplay loop>
      <source src="/videos/harmonic_response_2.mp4" type="video/mp4">
    Your browser does not support the video tag.
    </video>
  </center>
</div>

<p align="justify">
As we can observe from the animation, the magnitude of the vibration transmitted to the other end is decreased, and the vibration can be completely attenuated using an array.
</p>

<p align="justify">
The mechanism of Prof. Çetin Yılmaz obtains band gaps at low frequencies not by adding extra mass but by distributing the present mass and linking them together in a hinge mechanism. To illustrate the operating principle here is a simple system consisting of three point masses linked together by two rigid beams and a spring.
</p>

<center>
  <img src="/images/projects/me429_schema.png" alt="Schematic" style="width:55.0%;"/>
</center>

<p align="justify">
What happens is when the end points displace horizontally by an amount u, the middle point has to displace vertically by an amount u/tan&#952; due to geometry. As &#952; gets smaller, this vertical displacement gets very large. But a large displacement requires a large amount of energy which may not be present in the system. So in a way m_a limits the motion of the system by acting heavier than it is. This can be shown mathematically by solving the Lagrange's equation from which this equation of motion is obtained.
</p>

<center>
  <img src="/images/projects/me429_eom.png" alt="EOM" style="width:45.0%;"/>
</center>

<p align="justify">
Here, the term multiplying the acceleration term represents the effective inertia of the system. From here we can conclude that we can increase the effective inertia simply by decreasing &#952; and this is what inertial amplification refers to. For more details, please check out the <a href="https://journals.aps.org/prb/abstract/10.1103/PhysRevB.76.054309" target="_blank"> original paper</a>. 
</p>

<p align="justify">
Although this mechanism works well in the horizontal plane, it cannot support any load in the vertical direction (including its own weight). We designed a system and tested  it to make the mechanism operational in the vertical axis with minimum effect on the band gap. The following animation summarizes our work.
</p>
<div style="width:100%">
  <center>
    <video class="projectVideo" muted autoplay loop>
      <source src="/videos/me429_design.mp4" type="video/mp4">
    Your browser does not support the video tag.
    </video>
  </center>
</div>

<div style="width: 100%; height: 25px"></div>

<div style="width:100%" id="project-report">
  <center>
    <a href="/files/ME429_PROJECT_REPORT.pdf" download><img src="/images/projects/me429_report.PNG" style="width: 50%; object-fit: contain;" alt="Project Report"/></a>
  </center>
</div>