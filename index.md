---
layout: default
title: Junayed Ridwan
---

## About Me

<div class="about-layout">
<div class="about-photo">
	<img src="{{ "assets/images/profile-pic.jpg" | relative_url }}" alt="Profile Picture" class="profile-image">
</div>
<div class="about-copy">
<p><strong>Marine Robotics &amp; Systems Engineering:</strong> I have extensive experience designing robust mechanical systems for competitive environments. My past work includes engineering torpedo and dropper actuation mechanisms for autonomous underwater vehicles, as well as prototyping main hulls and 3D-printed thruster mounts for autonomous surface vessels.</p>

<p><strong>Simulation &amp; Analysis:</strong> I leverage industry-standard CAD and simulation software to take concepts from early models through rigorous Finite Element Analysis (FEA) and Computational Fluid Dynamics (CFD) long before they hit the manufacturing floor.</p>

<p><strong>Automotive Engineering (Current &amp; Future Work):</strong> I am currently expanding my portfolio into the automotive sector. I am applying my background in mechanical optimization to vehicle dynamics, custom hardware design, and performance modification projects.</p>

Explore <a href="{{ "/projects/" | relative_url }}">my projects</a>.
</div>
</div>

<section class="home-projects">
<h2>Projects</h2>
<div class="project-gallery">
		{% assign visible_projects = site.projects | where_exp: "project", "project.gallery != false" %}
		{% for project in visible_projects %}
			<div class="gallery-item">
				<a href="{{ project.url | relative_url }}">
					<img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
					<p>{{ project.title }}</p>
				</a>
			</div>
		{% endfor %}
</div>
</section>
