---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% include section.html %}

{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(?!pi$)" %}

{% include section.html background="images/background.jpg" dark=true %}

## Funding

Our work is made possible by funding from the following organizations.
{:.center}

{%
  include gallery.html

  image1="images/funding/nih.webp"
  link1="https://nih.gov/"
  tooltip1="National Institutes of Health"

  image2="images/funding/pelotonia.webp"
  link2="https://cancer.osu.edu/for-cancer-researchers/research/research-institutes-and-centers/pelotonia-institute-for-immuno-oncology"
  tooltip2="Pelotonia Institute for Immuno-Oncology"

  image3="images/funding/Ohio-State.webp"
  link3="https://idi.osu.edu/"
  tooltip2="Ohio State University Infectious Disease Institute"
%}
{:.center}