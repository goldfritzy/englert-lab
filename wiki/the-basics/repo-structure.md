---
description: A brief explanation of the folders and files in the website
---

# 🏗 Repo Structure

## Template vs. user content

The most important distinction to make is between **template content** ("under-the-hood") and **user content** (for your specific website).

**In general**, here's how the files and folders in the template fall into these two categories. We've tried to keep these as separated as possible, within the limitations of Jekyll.



| File Type   | User Content                                                                                                                                                                                                              | Template Content                                                                                                                                                                                                                                 |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Folders** | <p><code>/blog</code><br><code>/images</code><br><code>/team</code><br>etc. (starting with letters)<br><br><code>/_data</code></p><p><code>/_members</code></p><p><code>/_posts</code><br>(<code>_</code> exceptions)</p> | <p><code>github</code></p><p><code>.docker</code></p><p>etc. (starting with <code>.</code>)</p><p><br><code>_cite</code></p><p><code>_includes</code></p><p><code>_plugins</code></p><p>etc. (starting with <code>_</code>, except a few 👈)</p> |
| **Files**   | <p><code>_config.yaml</code> (top portion of file)</p><p><code>/_styles/-theme.scss</code><br><code>404.md</code><br><code>index.md</code><br><code>README.md</code></p>                                                  | <p><code>_config.yaml</code> (bottom portion of file)<br><code>.gitignore</code><br><code>CITATION.cff</code></p><p><code>Gemfile</code></p><p><code>Gemfile.lock</code><br><code>LICENSE.md</code></p>                                          |
|             |                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                  |

#### Template repo only content

There are a few files and folders that are needed for the `lab-website-template` repo itself, but don't belong in your generated/forked repo at all:

* `CHANGELOG.md`
* `testbed.md`
* `.github/ISSUE_TEMPLATE`
* `.github/workflows/versioning.yaml`
* `.github/pull_request_template.md` (rename `user_pull_request_template.md` in its place)

Keeping these files in your repo wont break anything per se, but they do increase clutter and confusion. The first time setup process automatically removes and renames these for you, but when updating your template version be sure not to accidentally re-add them to your repo.



### Images and Other Assets

The template comes with a default `/images` folder to hold all your site's images, but you can organize your images however you'd like. For example, you could put photos of your team in `/images/members/` and just refer to them like `images/members/jenglert.webp`.

You could also create `/videos` or any other folders you need for static assets and refer to them in the same way.

{% hint style="info" %}
The only exception to this is your [logo files](broken-reference) and [fallback image](broken-reference), which the template expects to be in `/images`.
{% endhint %}
