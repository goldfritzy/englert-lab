---
description: How to add, remove, and edit team members
---

# 🧑🤝🧑 Team Members

## Add/remove members

To add or remove a team member, create or delete a Markdown file in `/_members`.&#x20;

Each file will automatically generate its own page according to its filename. For example, a file with the name `tim-member.md` will generate a page at `/members/tim-member`.

{% hint style="info" %}
For ease of future updates, try to standardise a way of naming. For example, I have elected to use the first initial and the individuals last name. For example "jenglert"
{% endhint %}

{% hint style="info" %}
After adding members, you can display them on your site with the [list](broken-reference) and [portrait](broken-reference) components.
{% endhint %}

Example:

{% code title="jenglert.md" %}
```markdown
---
name: Joshua A. Englert, MD
image: images/members/jenglert.webp
role: pi
aliases:
  - J. Englert
  - J Englert
  - J. A. Englert
  - J A Englert
links:
  home-page: https://www.englertlab.com
  orcid: 0000-0002-1257-2239
---

A bio for Dr. Englert, written in Markdown.
A descriptions of his academic studies, his recent accomplishments, his goals for the future, his likes/dislikes, etc.
One or two paragraphs is probably best.
```
{% endcode %}

<table><thead><tr><th width="199">Parameter</th><th>Description</th></tr></thead><tbody><tr><td><code>name</code></td><td>Display name of team member.</td></tr><tr><td><code>image</code></td><td>URL to portrait photo of team member.</td></tr><tr><td><code>role</code></td><td>Team member's role in your organization. Determines the icon and default description text to show.<br><br>See <code>/_data/types.yaml</code> for what types of roles are built-in or to add your own.</td></tr><tr><td><code>description</code></td><td>Description of team member's role in your organization. Overrides any default text set from of  <code>role</code>.</td></tr><tr><td><code>aliases</code></td><td>By default, team member pages have a link at the bottom that goes to the "Research" page and searches for any papers by them. This field is a list of aliases/variations/abbreviations of the team member's name to search for.</td></tr><tr><td><code>links</code></td><td>Social media links for the team member, without any prefixes like <code>@</code>, <code>www.</code>, etc.<br><br>See <code>/_data/types.yaml</code> for what types of links are built-in or to add your own.</td></tr></tbody></table>

## Customize member page

The skeleton arrangement and style of team member pages are based on the `/_layouts/member.html` template, which you can freely edit to your liking.
