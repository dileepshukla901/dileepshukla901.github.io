---
layout: page
title: "Home"
class: home
---

# Hi, I'm Dileep Shukla

<div class="columns" markdown="1">

<div class="intro" markdown="1">
I'm a Lead Machine Learning Engineer providing consultancy for data-driven business solutions and managing end-to-end machine learning projects. I design and build data visualization, train, test & deploy ML & AI models for complex business problems across cloud and in-house infrastructures, utilizing both microservice and monolithic architectures.

In my previous role as a Lead ML Engineer at [Sprinklr](https://www.sprinklr.com/), I led a team of engineers and data scientists, focusing on Voice AI services such as TTS, ASR and Voice Analytics. Additionally, I worked on Reinforcement Learning problems for real time ads dynamic content optimizations, text-based models for insights, classification, and NER tasks, delivering impactful solutions that addressed critical business needs.

</div>

<div class="me" markdown="1">
<picture>
  <source srcset='/images/dileepshukla.webp' type='image/webp' />
  <img
    src='/images/dileepshukla.jpg'
    alt='Dileep Shukla'>
</picture>

{:.no-list}
* <a href="mailto:{{ site.email }}">{{ site.email }}</a>
</div>

</div>
I received my Master’s and Bachelor of Technology degrees from [IIT Kharagpur](https://www.iitkgp.ac.in/), majoring in Electrical Engineering.

During my college years, I interned at [DSP Investment Managers](https://www.dspim.com/), where I worked on customer churn prediction models. At [Times Internet](https://timesinternet.in/), I built Recommendation system for [Dineout](https://www.dineout.co.in). Details are in my [CV]({{ "/cv/" | relative_url }}).

## Featured <a href="{{ "/projects/" | relative_url }}">Projects</a>

<div class="featured-projects">
  {% assign sorted_projects = site.data.projects | sort: 'highlight' %}
  {% for project in sorted_projects %}
    {% if project.highlight %}
      {% include project.html project=project %}
    {% endif %}
  {% endfor %}
</div>

<a href="{{ "/projects/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show More Projects
</a>

<!-- ## Featured <a href="{{ "/publications/" | relative_url }}">Publications</a>

<div class="featured-publications">
  {% assign sorted_publications = site.publications | sort: 'year' | reverse %}
  {% for pub in sorted_publications %}
    {% if pub.highlight %}
      <a href="{{ pub.pdf }}" class="publication">
        <strong>{{ pub.title }}</strong>
        <span class="authors">{% for author in pub.authors %}{{ author }}{% unless forloop.last %}, {% endunless %}{% endfor %}</span>.
        <i>{% if pub.venue %}{{ pub.venue }}, {% endif %}{{ pub.year }}</i>.
        {% for award in pub.awards %}<br/><span class="award"><i class="fas fa-{% if award == "Best Paper Award" %}trophy{% else %}award{% endif %}" aria-hidden="true"></i> {{ award }}</span>{% endfor %}
      </a>
    {% endif %}
  {% endfor %}
</div>

<a href="{{ "/publications/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show All Publications
</a> -->
