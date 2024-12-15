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


## Courses, Hackathons, Certificates and others

{% for cc in site.data.courses_certificates %}
{% include cv/courses_certificates.html cc=cc %}
{% endfor %}


I authorize the processing of the personal data contained in my curriculum vitae in accordance with Article 13 of Legislative Decree 196/2003 and Article 13 of EU Regulation 2016/679 on the protection of individuals with regard to the processing of personal data.



[cv]: {{ site.url }}/files/cv.pdf "My CV."

[github]: https:/www.github.com/Giovo17 "github.com/Giovo17"



