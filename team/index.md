---
title: Team
nav:
  order: 3
  tooltip: About our team
carousels:
  - images: 
    - image: /images/funding/ats.webp
    - image: /images/funding/csctr.webp
    - image: /images/funding/feds.webp
    - image: /images/funding/nhlbi.webp
    - image: /images/funding/osucom.webp
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


{% include carousel.html height="25" unit="%" duration="10" number="1" %}

{:.center}