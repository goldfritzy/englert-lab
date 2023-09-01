---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---
# {% include icon.html icon="fa-regular fa-envelope" %}Contact
## Interested in our Lab?


Dr. Englert is can be contacted at his email or through Twitter.

{%
  include button.html
  type="email"
  text="joshua.englert@osumc.edu"
  link="joshua.englert@osumc.edu"
%}

{%
  include button.html
  type="external"
  text="Follow Dr. Englert on Twitter!"
  link="https://twitter.com/joshenglert_md"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col2 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col3 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
