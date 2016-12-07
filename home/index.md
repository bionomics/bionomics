---
layout: page
title:
excerpt: "Workshop on the biology and economics of mutualisms being held at the Max Planck Institute for Evolutionary Biology"
---

### The Biology and Economics of Mutualisms Workshop

## 1st - 3rd November 2017

Mutualisms---between-species interactions beneficial to all organisms involved---are at the heart of many thriving ecosystems.
The objective of this workshop is to present the latest developments in the evolution of mutualisms and to demonstrate the important role played by interdisciplinary approaches drawing from economic theory in the study of such systems.

---

# Important dates

**31 March 2017** Deadline for submission for short-talks and registration

**31 April 2017** Notification of acceptance

---

<!-- We are now welcoming submissions for short talks.
Submissions should include name, affiliation, title of the talk, abstract (of no more than 250 words).
Please send the submissions to mutual-workshop@evolbio.mpg.de.
Registration fees will cover food and accommodation for the complete duration of the conference. -->

We will be welcoming submissions for short talks from the **1st January 2017**.
Submissions should include `name, affiliation, title of the talk, abstract (of no more than 250 words)`.
Email address for submission and further details regarding *nominal registration fees* will be posted in January 2017.
In the meantime if you have any queries, feel free to contact the organisers.

{% capture site_tags %}{% for tag in site.tags %}{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tags_list = site_tags | split:',' | sort %}

<ul class="tag-box inline">
  {% for item in (0..site.tags.size) %}{% unless forloop.last %}
    {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
    <li><a href="#{{ this_word }}">{{ this_word }} <span>{{ site.tags[this_word].size }}</span></a></li>
  {% endunless %}{% endfor %}
</ul>

{% for item in (0..site.tags.size) %}{% unless forloop.last %}
  {% capture this_word %}{{ tags_list[item] | strip_newlines }}{% endcapture %}
  <h2 id="{{ this_word }}">{{ this_word }}</h2>
  <ul class="post-list">
  {% for post in site.tags[this_word] %}{% if post.title != null %}
    <li><a href="{{ site.url }}{{ post.url }}">{{ post.title }}<span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></li>
  {% endif %}{% endfor %}
  </ul>
{% endunless %}{% endfor %}

<!-- # Keynote speakers

[Erol Akçay](https://erolakcay.wordpress.com/) (University of Pennsylvania)

[Michelle Afkhami](https://michelleafkhami.wordpress.com/) (University of Miami)

[Megan Frederickson](http://mutualism.ca/) (University of Toronto)

[Olivia Roth](http://www.geomar.de/en/mitarbeiter/fb3/ev/oroth/) (GEOMAR Helmholtz Centre for Ocean Research Kiel)

[Claire Spottiswoode](http://www.africancuckoos.zoo.cam.ac.uk/index.html) (University of Cambridge)


# Confirmed short-talk speakers

[Judie Bronstein](http://www.eebweb.arizona.edu/faculty/bronstein/Bronstein_Lab/HOME.html) (University of Arizona)

[Redouan Bshary](https://www.unine.ch/ethol/home/team/bshary-redouan.html) (University of Neuchâtel)

[Peter Hammerstein](https://www.biologie.hu-berlin.de/en/gruppenseiten-en/sfb618/people/hammerstein_peter) (Humboldt University of Berlin)

[Christoph Hauert](http://www.math.ubc.ca/~hauert/) (University of British Columbia)

[John McNamara](http://www.bristol.ac.uk/maths/people/john-m-mcnamara/index.html) (University of Bristol)

[Georg Nöldeke](https://sites.google.com/site/georgnoldeke/) (University of Basel)

[Ronald Noë](https://sites.google.com/site/ronaldnoe/) (University of Strasbourg)

[Naomi Pierce](http://piercelab.oeb.harvard.edu/) (Harvard University) -->


# Organisers

[Chaitanya S. Gokhale](http://gokhalechaitanya.github.io/) (Max Planck Institute for Evolutionary Biology)

[Jorge Peña](https://jorgeapenas.wordpress.com/) (GEOMAR Helmholtz Centre for Ocean Research Kiel)
