---
layout: cv
title: CV
permalink: cv/
jsarr:
- js/scripts.js
---
<h1 id="cv-title"><a href="{{ site.url }}">Giovanni Spadaro</a></h1>


<p id="cv-subtitle"><i>Data Science master student</i></p>

<div class="cv-spacer"></div>

<div class="cv-image-links-wrapper">
	<div class="cv-image-links">
		{% for link in site.data.social-links %}
			{% if link.cv-group == 1 %}
				{% include cv-social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
	<div class="cv-image-links">
		{% for link in site.data.social-links %}
			{% if link.cv-group == 2 %}
				{% include cv-social-link.html link=link %}
			{% endif %}
		{% endfor %}
	</div>
</div>

***

## Education

{::nomarkdown}
{% for degree in site.data.education %}
{% include cv/degree.html degree=degree %}
{% endfor %}
{:/}


## Academic Research Experience

{% for experience in site.data.experiences %}
{% if experience.type == 'academic' %}
{% include cv/experience.html experience=experience %}
{% endif %}
{% endfor %}


## Courses and Certificates

{% for cc in site.data.courses_certifications %}
{% include cv/courses_certificates.html cc=cc %}
{% endfor %}


[cv]: {{ site.url }}/files/cv.pdf "My CV."

[github]: https:/www.github.com/Giovo17 "github.com/Giovo17"



