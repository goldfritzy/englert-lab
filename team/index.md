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

  image1="images/funding/ats.webp"
  link1="https://www.thoracic.org/"
  tooltip1="American Thoracic Society"

  image2="images/funding/csctr.webp"
  link2="https://www.csctr.org"
  tooltip2="Central Society for Clinical and Translational Research"

  image3="images/funding/feds.webp"
  link3="https://www.defense.gov/"
  tooltip3="The United States Department of Defense"

  image4="images/funding/nhlbi.webp"
  link4="https://www.nhlbi.nih.gov/"
  tooltip4="National Heart, Lung, and Blood Institute"
  
  image5="images/funding/osucom.webp"
  link5="https://www.medicine.osu.edu/"
  tooltip5="The Ohio State University College of Medicine"
%}
{:.center}