---
layout: page
title: Participants
participants:
  - name: Reymond Akpanya
    affiliation: RWTH Aachen
    links:
      "GitHub: ReymondAkpanya": https://github.com/ReymondAkpanya

  - name: Frank Lübeck
    affiliation: RWTH Aachen
    links:
      "GitHub: frankluebeck": https://github.com/frankluebeck

  - name: Jens Brandt
    affiliation: RWTH Aachen
    links:
      "GitHub: flyingapfopenguin": https://github.com/flyingapfopenguin

  - name: Mun See Chang
    affiliation: University of St Andrews
    links:
      "GitHub: Munsee": https://github.com/Munsee

  - name: Deepshikha Chatterjee
    affiliation: Ambedkar University Delhi

  - name: Leila Ghanbari Maman
    affiliation: University of Tehran

  - name: Tom Görtzen
    affiliation: RWTH Aachen
    links:
      "GitHub: TomGoertzen": https://github.com/TomGoertzen

  - name: Ruth Hoffmann
    affiliation: University of St Andrews
    links:
      "GitHub: ruthhoffmann": https://github.com/ruthhoffmann

  - name: Max Horn
    affiliation: TU Kaiserslautern
    links:
      "GitHub: fingolfin": https://github.com/fingolfin

  - name: Ali Iranmanesh
    affiliation: Tarbiat Modares University

  - name: Christopher Jefferson
    affiliation: University of St Andrews
    links:
      "GitHub: ChrisJefferson": https://github.com/ChrisJefferson

  - name: Fatemeh Koorepazan-Moftakhar
    affiliation: Comenius University in Bratislava

  - name: Anna Limbach
    affiliation: RWTH Aachen

  - name: Dominika Mihálová
    affiliation: Comenius University in Bratislava

  - name: Kuroš Mavaddat Nežâd
    affiliation: University of Kashan

  - name: Alice Niemeyer
    affiliation: RWTH Aachen
    links:
      "GitHub: aniemeyer": https://github.com/aniemeyer

  - name: Daniel Rademacher
    affiliation: RWTH Aachen
    links:
      "GitHub: danielrademacher": https://github.com/danielrademacher

  - name: Friedrich Rober
    affiliation: RWTH Aachen
    links:
      "Github: FriedrichRober": https://github.com/FriedrichRober

  - name: Leonard Soicher
    affiliation: Queen Mary University of London
    links:
      "GitHub: lhsoicher": https://github.com/lhsoicher

  - name: Anna Sucker
    affiliation: RWTH Aachen
    links:
      "GitHub: AnnaKDS": https://github.com/AnnaKDS

  - name: Vinay Vilas Wagh
    affiliation: Indian Institute of Technology Guwahati

  - name: Bardia Jahangiri
    affiliation: University of Kashan

  - name: Mohammad Moein Yousefian Arani
    affiliation: University of Kashan

  - name: Meike Weiß
    affiliation: RWTH Aachen
    links:
      "GitHub: MeikeWeiss": https://github.com/MeikeWeiss

  - name: Lucas Wollenhaupt
    affiliation: RWTH Aachen
    links:
      "GitHub: wucas": https://github.com/wucas

  - name: Wilf Wilson
    links:
      "GitHub: wilfwilson": https://github.com/wilfwilson
      
  - name: Eileen X. Pan
    affiliation: Warwick--Monash Alliance
    links:
      "GitHub: xpan-eileen": https://github.com/xpan-eileen
---

<ol>{% assign participants = page.participants | sort: "name" %}
{% for p in participants %}
  <li>
    <strong>{{ p.name }}</strong>
    {% if p.affiliation != null %} ({{ p.affiliation }}){% endif %}
    {% if p.links != null %}
        {% for item in p.links %}
            <a href="{{ item[1] }}">({{ item[0] }})</a>
        {% endfor %}
    {% endif %}
    <br/>
      {% if p.talk != null %} Talk: {{ p.talk }}{% endif %}
  </li>
{% endfor %}
</ol>

{% if site.data.feedback.size > 0 %}

<ul>
{% for p in site.data.feedback %}
  <li>
    <strong>{{ p.name }}</strong>
    {% if p.package != null %} (author of {{ p.package }}){% endif %}
    <br/>
    {% if p.feedback != null %} {{ p.feedback }}{% endif %}
  </li>
{% endfor %}
</ul>

{% endif %}
