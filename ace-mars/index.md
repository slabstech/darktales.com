---
layout: page
title: ACE-MARS
excerpt: 'Autonomous Construction Engineering in Mars Environment'
search_omit: true
---

Autonomous Construction Engineering in Mars Environment

* Objective : Occupy Mars

* Use Case : How will humans settle in a hostile environment ?

That's where "ACE-MARS" come to the picture, building the basic blocks for survival.

* History : Relive the Space Race since Sputnik in 21st century

* SOA : Starship, New Shepard, Mangalyaan, Chinese Mission

* Ideas

  * Wall Prefabrication & Setup

  * Solar Rooftop : Transmission and installation

  * 3D printing - cutting edge, brick & kiln low cost using existing

  * Block Extraction - hyperloop, boring company by elon musk

  * Underground Travel

  * Survey for Land
    * Exploration
    * Nutrient/Soil Testing

  * Map of Mars
    * Current Active Robots
    * Previous Landed Robots
    * Max. Solar Irradiation
    * Water Exploration - possible ways of collections

  * Swarm Machines
    * Send them a year ahead of human arrival and build critical infrastructure.
      * for Human Habitation
      * Solar Panels - Power Generation
      * Underground Travel
      * Mineral Extraction & Geothermal Extraction
      * Terrestrial exploration and formation
      * Communication Development
        * Old Style - Mirror & Radios
        * Till next batch of experiments arrive for satellite deployment
      * Landing Pads Creation

* Planning
  * City planning and Zoning, Starting from a clean slate from Sim City
  * Mapping Terrain and Weather Conditions
  * Transportation for workers, engineers
  * Energy Generation & Transmission
  * Local resources exploration for in-situ development.

### Additional Detail Information

<ul class="post-list">
{% for post in site.categories.ace-mars %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
