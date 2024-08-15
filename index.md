---
layout: workshop
venue: "University at Buffalo, SUNY"   # brief name of host site without address (e.g., "Euphoric State University")
address: "University at Buffalo, SUNY, North Campus, Natural Sciences Complex"   # full street address of workshop (e.g., "Room A, 123 Forth Street, Blimingen, Euphoria")
country: "United States"      # lowercase two-letter ISO country code such as "fr" (see https://en.wikipedia.org/wiki/ISO_3166-1#Current_codes)
language: "en"     # lowercase two-letter ISO language code such as "fr" (see https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
latitude: "43.002890"     # decimal latitude of workshop venue (use https://www.latlong.net/)
longitude: "-78.788780"    # decimal longitude of the workshop venue (use https://www.latlong.net)
humandate: "August 15-16, 2024"    # human-readable dates for the workshop (e.g., "Feb 17-18, 2020")
humantime: "09:00 am - 5:00 pm EDT"    # human-readable times for the workshop (e.g., "9:00 am - 4:30 pm")
startdate: 2024-08-15      # machine-readable start date for the workshop in YYYY-MM-DD format like 2015-01-01
enddate: 2022-08-16        # machine-readable end date for the workshop in YYYY-MM-DD format like 2015-01-02
organizers: ["Alexey Akimov", "Mohammad Shakiba", "Daeho Han" ] # boxed, comma-separated list of instructors' names as strings, like ["Kay McNulty", "Betty Jennings", "Betty Snyder"]
helper: [ ] # boxed, comma-separated list of helpers' names, like ["Marlyn Wescoff", "Fran Bilas", "Ruth Lichterman"]
email: ["alexeyak@buffalo.edu"]    # boxed, comma-separated list of contact email addresses for the host, lead instructor, or whoever else is handling questions, like ["marlyn.wescoff@example.org", "fran.bilas@example.org", "ruth.lichterman@example.org"]
collaborative_notes:   # optional: URL for the workshop collaborative notes, e.g. an Etherpad or Google Docs document (e.g., https://pad.carpentries.org/2015-01-01-euphoria)
googleform: 
carpentry: "sc"
---


{% comment %}
root: .  # Is the only page that doesn't follow the pattern /:path/index.html
permalink: index.html  # Is the only page that doesn't follow the pattern /:path/index.html
{% endcomment %}


# MolSSI workshop: "Machine-Learning in Quantum and Nonadiabatic Dynamics", 2024

## Description

Quantum dynamics and nonadiabatic molecular dynamics (NA-MD) simulations can provide comprehensive insights into many 
photophysical and photochemical processes in a broad class of materials and natural systems. However, the complexity of such methods that
comes both from the exponential scaling due to the multitude of wavepacket branching outcomes and from the steep computational demands 
of the underlying electronic structure calculations makes prohibitively expensive, especially when applied to nanoscale or periodic systems. 
Recently, machine-learning (ML) techniques have revolutionized various branches of computational chemistry and simulated the development 
of new approaches to handle complexity of quantum or quantum-classical simulation methods, study nanoscale systems, and investigate long 
timescale dynamics. Several seemingly-disjoint sub-communities of computational chemistry, such as "electronic structure", "quantum/nonadiabatic 
dynamics", and "materials", all utilize a broad spectrum of specialized ML techniques. However, the unified underlying formalism of ML-based 
methods implies that the techniques and software developed by one of these groups may be re-used by the other groups. Exchanging the accumulated 
experiences, best practices, and developed software has a great potential to stimulate further progress in each of the identified fields. 
Breaking the inter-disciplinary boundaries of the sub-communities and unifying them through their shared interest in the ML can lead to 
new ideas and solutions.

This workshop will facilitate the exchange of ideas and promote the adoption of existing and developing software in the field of 
Quantum and Nonadiabatic dynamics. It aims to help the community experts to get a better awareness of the existing developments. 
The workshop is a melting pot of experts working in one of the three branches: (1) ML-centric material research chemistry practitioners; 
(2) electronic structure ML practitioners; (3) quantum/nonadiabatic dynamics ML practitioners. It is our expectation that all these groups
 will be able to "educate" each other, disseminate and promote the best practices and tools, and raise the present-day challenges they face.


## Logistics

{% if page.humandate %}
<p id="when">
  <strong>When:</strong>
  {{page.humandate}}.
  {% include workshop_calendar.html %}
</p>
{% endif %}

{% if page.latitude and page.longitude %}
<p id="where">
  <strong>Where:</strong>
  {{page.address}}.
  Get directions with
  <a href="//www.openstreetmap.org/?mlat={{page.latitude}}&mlon={{page.longitude}}&zoom=16">OpenStreetMap</a>
  or
  <a href="//maps.google.com/maps?q={{page.latitude}},{{page.longitude}}">Google Maps</a>.
</p>
{% endif %}

{% comment %}
CONTACT EMAIL ADDRESS
Display the contact email address set in the configuration file.
{% endcomment %}
<p id="contact">
  <strong>Contact</strong>:
  Please email
  {% if page.email %}
  {% for email in page.email %}
  {% if forloop.last and page.email.size > 1 %}
  or
  {% else %}
  {% unless forloop.first %}
  ,
  {% endunless %}
  {% endif %}
  <a href='mailto:{{email}}'>{{email}}</a>
  {% endfor %}
  {% else %}
  to-be-announced
  {% endif %}
  for more information.
</p>


## Schedule
{% include base_path.html %}

### August 14, 2024, Wednesday

 Arrivals and Welcome dinner.

### August 15, 2024, Thursday: Day 1

|       Time           |       Name       |         Topic                            |
|----------------------|------------------|------------------------------------------|
|  9:00 am -  9:15 am  | Alexey Akimov    | Introductory remarks                     |
|  9:15 am - 10:00 am  | Daniel Crawford  | MolSSI presentation                      |
| 10:00 am - 10:40 am  | Zhenggang Lan (remote)  | Research presentation             |
| 10:40 am - 11:20 am  | Maksim Kulichenko | Research presentation         |
| 11:20 am - 12:00 am  | Rafael Gomez-Bombarelli (remote)  | Research presentation            |
| Noon -      1:30 pm  | |  Lunch break |
|  1:30 pm -  2:10 pm  | Michele Pavanello  | Research presentation                  |
|  2:10 pm -  2:50 pm  | Mark Tuckerman  | Research presentation  | 
|  2:50 pm -  3:30 pm  | Nitin Murthy (Johannes Hachmann group)     |
|  3:30 pm -  4:10 pm  | Mohammad Shakiba (Alexey Akimov group)  | Research presentation      |
|  4:10 pm -  5:00 pm  |   | Discussions      |


### August 16, 2024, Friday: Day 2

|       Time           |       Name       |         Topic                            |
|----------------------|------------------|------------------------------------------|
|  9:00 am -  9:40 am  | Pavlo Dral (remote)  | Research presentation                |
|  9:40 am - 10:20 am  | Linjun Wang (remote)  | Research presentation                 |
| 10:20 am - 11:00 am  | Xiang Sun (remote)  | Research presentation                    |
| 11:00 am - 11:40 am  | Alexei Kananenka   | Research presentation             |
| 11:40 am - 12:00 am  |   | Discussions         |
| Noon -      1:30 pm  | |  Lunch break |
|  1:30 pm -  2:10 pm  | Alexey Akimov  | Research presentation         |
|  2:10 pm -  2:50 pm  | Oleg Prezhdo  | Research presentation         |
|  2:50 pm -  3:30 pm  | Dmitri Kilin  | Research presentation         |
|  3:30 pm -  4:10 pm  | Johannes Hachmann (remote)  | Research presentation      |
|  4:10 pm -  5:50 pm  |   | Closing remarks. Discussions      |

### August 17, 2024, Saturday

 Departures.


### Acknowledgement

This workshop is made possible by the NSF MolSSI program. Thank you!


{% include links.md %}
