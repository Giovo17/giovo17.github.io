---
layout: page
title: Dissemination
permalink: dissemination/
---


My scientific dissemination events.


## Talk

My dissertation contributed interactive interfaces to enable machine learning interpretability at scale and for everyone.

<div class="cover-wrapper cover-wrapper-1-col l-text">
	{% include dissertation/document.html details=false location=home %}
</div>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.dissertation == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<div class="project-spacer-small"></div>

## Research

Research publications for fans of human-computer interaction, data visualization, and machine learning.

<div class="project-spacer-small"></div>

<div class="l-page project-grid">
    {% for project in site.categories.papers %}
    {% include project.html project=project %}
    {% endfor %}
</div>

<div class="project-spacer"></div>

## Interactive Articles

Enhanced reading experiences that demonstrate what's possible when dynamic media are effectively combined.

<div class="project-spacer-small"></div>

<div class="cover-wrapper cover-wrapper-2-col l-middle">
	{% assign sortedArticles = site.data.articles | where: "featured", true %}
	{% assign ia = site.categories.papers | where:"permalink", "papers/interactive-articles" %}

	{% assign feature = sortedArticles[0] %}
	{% include feature.html feature=feature %}

	{% assign feature = ia[0] %}
	{% include feature.html feature=feature %}
</div>

<div class="project-spacer-small"></div>

<ul>
    {% for article in site.data.articles %}
        {% unless article.feature-only %}
            <li><a href="{{ article.url }}" style="text-transform: capitalize">{{ article.title }}</a> <small style="color: #c0c0c0">{{ article.year }}</small></li>
        {% endunless %}
    {% endfor %}
</ul>

<div class="project-spacer-small"></div>

