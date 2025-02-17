---
layout: home
title: Home
---
<div id="intro-wrapper" class="l-text">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="/images/portrait.jpeg"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Hi, I'm Giovanni</h1>
			<div id="intro-subtitle">Data Science master student @ UNICT</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<!-- <hr class="l-middle home-hr"> -->
	<div id="everything-else" class="l-middle">
		
		<!-- <a href="{{ site.url }}/dissemination"><div><i class="fa fa-chalkboard-user icon icon-right-space"></i>Teaching</div></a> -->

		<!-- <a href="{{ site.url }}/blog"><div><i class="fa fa-chalkboard-user icon icon-right-space"></i>Blog</div></a> -->
		<!-- <a href="{{ site.url }}/teaching"><div><i class="fa fa-chalkboard-user icon icon-right-space"></i>Teaching</div></a> -->
		<!-- <a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a> -->
		<!-- <a href="{{ site.url }}/everything-else"><div><i class="fa fa-list-ul icon icon-right-space"></i>Everything Else</div></a> -->
		
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		
	</div>
	<div style="height: 1rem"></div>
	<h1>Site under construction</h1>
	<div style="height: 1rem"></div>
	<div>
	Computer Engineer, master student in Data Science at University of Catania, private professor, ML research enthusiast and applied AI solutions lover.
	</div>

</div>


